NPM?=	npm
NPX?=	npx
D2?=	d2
MINTLIFY=	$(NPX) mintlify
PRETTIER=	$(NPX) prettier

PORT?=	3333

D2_FILES=	$(shell find images -name '*.d2')
SVG_FILES=	$(D2_FILES:%.d2=%.svg)
MDX_FILES=	$(wildcard **/*.mdx)
JSON_FILES=	mint.json package.json

.PHONY: all
all: $(SVG_FILES) fmt

.PHONY: start
start: $(SVG_FILES)
	$(MINTLIFY) dev --port $(PORT)

.PHONY: fmt
fmt:
	$(PRETTIER) --write $(MDX_FILES) $(JSON_FILES)
	$(D2) fmt $(D2_FILES)

.PHONY: check
check:
	$(PRETTIER) --check $(MDX_FILES) $(JSON_FILES)
	$(MINTLIFY) broken-links

$(SVG_FILES): $(D2_FILES)
	$(D2) --theme=300 --dark-theme=200 $< $@

