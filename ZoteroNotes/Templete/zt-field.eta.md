<% if(it.title) { -%>
title: "<%= it.title %>"
<% } -%>
<% if(it.authors.first()) { -%>
authors:
<% it.authors.forEach(author => { -%>
  - <%= author %>
<% })}  -%>
<% if(it.date) { -%>
publish-date: <%= it.date %>
<% } -%>
import-date: <%= it.dateAccessed %>
<% if(it.ISBN) { -%>
ISBN: <%= it.ISBN %>
<% } -%>
<% if(it.citekey) { -%>
citekey: "<%= it.citekey %>"
<% } -%>
<% if(it.tags.first()) { -%>
tags:
<% it.tags.forEach(tag => { -%>
  - <%= tag %>
<%- })} %>