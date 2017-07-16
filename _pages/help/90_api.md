---
layout: page
title: Programmers API
permalink: /help/api/
tags: helppage
---

## Introduction

This page explains how programmers can make other websites and software interact with FYI via an "API".

FYI does not have a full API yet, but we are gradually adding lots of things that are similar in use to an API as they are requested.

## Linking to new requests

To encourage your users to make links to a particular public authority, use URLs of the form [https://fyi.org.nz/new/auckland_council](https://fyi.org.nz/new/auckland_council). These are the parameters you can add to those URLs, either in the URL or from a form.

*   **title** - default summary of the new request.
*   **default_letter** - default text of the body of the letter. The salutation (Dear...) and signoff (Yours...) are wrapped round this.
*   **body** - as an alternative to default_letter, this sets the default entire text of the request, so you can customise the salutation and signoff.
*   **tags** - space separated list of tags, so you can find and link up any requests made later, e.g. _openlylocal spending_id:12345_. The : indicates it is a machine tag. The values of machine tags may also include colons, useful for URIs.

## RSS (actually, Atom) feeds

There are Atom feeds on most pages which list OIA requests, which you can use to get updates and links in XML format. Find the URL of the Atom feed in one of these ways:

*   Look for the ![Feed-16](/assets/feed-16-cb3420750747d3e9acd1086359fdeec7.png) RSS feed links.
*   Examine the `<link rel="alternate" type="application/atom+xml">` tag in the head of the HTML.
*   Add `/feed` to the start of another URL.

In particular, even complicated search queries have Atom feeds. You can do all sorts of things with them, such as query by authority, by file type, by date range, or by status. See the [advanced search tips](https://fyi.org.nz/search) for details.

## JSON structured data

Quite a few pages have JSON versions, which let you download information about objects in a structured form. Find them by:

*   Adding `.json` to the end of the URL.
*   Look for the `<link rel="alternate" type="application/json">` tag in the head of the HTML.

Requests, users and authorities all have JSON versions containing basic information about them. Every Atom feed has a JSON equivalent, containing information about the list of events in the feed.

## Spreadsheet of all authorities

A spreadsheet file listing every body in FYI is available: [all-authorities.csv](https://fyi.org.nz/body/all-authorities.csv)

## More help

Please [contact us](https://fyi.org.nz/help/contact) if you need an API feature that isn't there yet. It's very much a work in progress, and we do add things when people ask us to.
