---
layout: intern
title: Tables
description: Tables template.
permalink: /docs/4.0/pages/tables
---

<div class="table-wrapper">
  <div class="table-scroller dragscroll">
    <table class="table">
      <thead class="thead thead-light">
        <tr>
          <th>
            <div class="cell-inner">
              <div class="custom-control custom-checkbox custom-checkbox-alone">
                <input type="checkbox" class="custom-control-input" id="thead">
                <label class="custom-control-label" for="thead"></label>
              </div>
            </div>
          </th>
          <th><div class="cell-inner">Nom</div></th>
          <th><div class="cell-inner">Type</div></th>
          <th><div class="cell-inner">Vers</div></th>
          <th><div class="cell-inner">Agent</div></th>
          <th><div class="cell-inner">Mise à jour</div></th>
          <th></th>
        </tr>
      </thead>
      <tbody class="tbody">
        {% for item in site.data.tables %}
        <tr>
          <td>
            <div class="cell-inner">
              <div class="custom-control custom-checkbox custom-checkbox-alone">
                <input type="checkbox" class="custom-control-input" id="thead">
                <label class="custom-control-label" for="thead"></label>
              </div>
            </div>
          </td>
          <td><div class="cell-inner">{{ item.name }}</div></td>
          <td><div class="cell-inner">{{ item.type }}</div></td>
          <td><div class="cell-inner">{{ item.version }}</div></td>
          <td><div class="cell-inner">{{ item.agent }}</div></td>
          <td><div class="cell-inner">{{ item.update }}</div></td>
          <td>
            <div class="cell-inner">
              <button class="btn btn-only-icon btn-transparent btn-favorite">
                <span class="sr-only">Favorite</span>
                <i class="icons-favorite-on icon-size-1x25"></i>
              </button>
              <button class="btn btn-only-icon btn-transparent btn-color-gray">
                <span class="sr-only">Favorite</span>
                <i class="icons-divers icon-size-1x25"></i>
              </button>
              <div class="btn-group dropdown">
                <button class="btn btn-only-icon btn-transparent btn-color-gray" type="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false" data-boundary="window">
                  <span class="sr-only">Favorite</span>
                  <i class="icons-options icon-size-1x75"></i>
                </button>
                <div class="dropdown-menu dropdown-menu-right">
                  <button type="button" class="dropdown-item" href="#">Télécharger</button>
                  <button type="button" class="dropdown-item" href="#">Imprimer</button>
                  <button type="button" class="dropdown-item" href="#">Partager</button>
                </div>
              </div>
            </div>
          </td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
</div>