NPM?=	npm
NPX?=	npx
MINTLIFY=	$(NPX) mintlify
PRETTIER=	$(NPX) prettier

PORT?=	3333


SRC=	$(wildcard **/*.mdx) mint.json package.json

.PHONY: start
start:
	$(MINTLIFY) dev --port $(PORT)

.PHONY: fmt
fmt:
	$(PRETTIER) --write $(SRC)

.PHONY: check
check:
	$(PRETTIER) --check $(SRC)
	$(MINTLIFY) broken-links

