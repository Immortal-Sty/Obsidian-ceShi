[!note] [Page <%= it.pageLabel %>]
<%- if (it.backlink) { -%>
(<%= it.backlink %>)
<%- } %>

<%= it.imgEmbed %><%= it.text.replace(/[\r\n]+/g, "\n\n") %>
<% if (it.comment) { %>
---

<%= it.comment %>
<% } %>