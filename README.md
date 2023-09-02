<p align="center">
    <picture>
        <source media="(prefers-color-scheme: dark)" srcset="images/logo/dark.svg"/>
        <img alt="Defer logo" src="images/logo/light.svg"/>
    </picture>
</p>
<p align="center">
    Zero infrastructure Node.js background jobs
</p>
<p align="center">
    <a href="https://docs.defer.run/">Documentation</a>
    <span>&nbsp;·&nbsp;</span>
    <a href="https://www.defer.run/blog">Blog</a>
    <span>&nbsp;·&nbsp;</span>
    <a href="https://discord.gg/x2v84Vqsk6">Community</a>
    <span>&nbsp;·&nbsp;</span>
    <a href="https://github.com/defer-run/defer.client/discussions/categories/roadmap">Roadmap / RFCs</a>
</p>
<br/>

## Introduction

This repository contains the documentation of Defer. The documentation
is built and deployed using [Mintlify](https://mintlify.com/).

## Quickstart

Install dependencies with:

	npm ci
	
Start local server with:

	make start
	
Format `.json` and `.mdx` files with:

	make fmt

Check formatting and broken links with:

	make check
