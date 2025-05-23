---
# This page was generated from the add-on.
title: Dev Add-On
type: userguide
weight: 1
cascade:
  addon:
    id: dev
    version: 0.10.0
---

# Dev Add-On

An add-on to help with development of ZAP. It starts a simple test web service, which by default will be accessible via http://localhost:9091


It provides:

## API Pages

Two simple OpenAPI specs, both of which require no authentication. One of the APIs described by the specs can only be accessed when authenticated.

## Authentication Pages

A growing set of authentication pages, for use in testing ZAP authentication handling.

## CSRF Pages

A set of pages with forms and CSRF tokens that are checked on POST requests.

## HTML Pages

A set of pages which store various types of data in localStorage and sessionStorage.

## Sequence Pages

A set of pages for testing the sequence add-on.
