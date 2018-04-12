---
layout: docs
title: Navbar
description: Documentation and examples for Bootstrap's powerful, responsive navigation header, the navbar. Includes support for branding, navigation, and more, including support for our collapse plugin.
group: components
toc: true
permalink: /docs/4.0/components/navbar
---

{% example html %}
<header class="mastheader">
  <div class="mastheader-logo">
    <a href="/docs">
      <span class="sr-only">SNCF</span>
      <img alt="SNCF" src="{{ site.baseurl }}/assets/img/brand/sncf-logo.png" width="70" />
    </a>
  </div>
  <h1 class="mastheader-title d-none d-xl-block text-uppercase text-white pt-2 pl-3 mb-0">Nom application</h1>
  <div class="mastheader-search pr-md-4 pl-md-4" data-component="searchbar">
    <label class="font-weight-medium text-white pr-3 mb-0">Rechercher</label>
    <div class="input-group align-items-center">
      <div class="form-control-container" data-component="control" data-clear-option="true">
        <input type="text" class="form-control clear-option" data-role="input" data-placeholder="Rechercher" />
        <span class="form-control-state"></span>
        <button type="button" class="btn-clear btn-primary d-none" data-btn="clear">
          <span class="sr-only">Clear text</span>
          <i class="icons-close"></i>
        </button>
      </div>
      <div class="input-group-append input-group-last">
        <button type="button" class="btn btn-primary btn-only-icon">
          <i class="icons-search"></i>
        </button>
      </div>
      <button type="button" class="btn btn-only-icon btn-white d-block d-md-none" data-role="close"><i class="icons-close icon-size-1x25"></i></button>
    </div>
  </div>
  <ul class="mastheader-toolbar toolbar mb-0">
    <li class="toolbar-item d-none d-md-block">
      <a href="#" class="btn btn-only-icon btn-notif toolbar-item-spacing">
        <span class="sr-only">Alert</span>
        <i class="icons-alert-underline icon-size-1x25 icon-size-md-1x50"></i>
        <span class="notif">1</span>
      </a>
    </li>
    <li class="toolbar-item no-separator d-block d-md-none">
      <a href="#" class="btn btn-only-icon toolbar-item-spacing" data-component="searchbar-toggle">
        <span class="sr-only">Open search</span>
        <i class="icons-search icon-size-1x25 icon-size-md-1x50"></i>
      </a>
    </li>
    <li class="toolbar-item">
      <div class="btn-group dropdown">
        <button class="btn btn-transparent dropdown-toggle toolbar-item-spacing" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          <i class="icons-account-offline icon-size-1x25 icon-size-md-1x50 mr-xl-2"></i>
          <span class="d-none d-xl-block">Pierre Dumont</span>
          <i class="icons-arrow-down d-none d-xl-block"></i>
        </button>
        <div class="dropdown-menu dropdown-menu-right" aria-labelledby="dropdownMenuButton">
          <a class="dropdown-item" href="#">Paramètre du compte</a>
          <a class="dropdown-item" href="#">Préférences</a>
          <a class="dropdown-item" href="#">Se déconnecter</a>
        </div>
      </div>
    </li>
  </ul>
</header>
{% endexample %}