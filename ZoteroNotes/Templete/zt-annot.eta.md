[!quote] [Page <%= it.pageLabel %>]
<%- if (it.backlink) { -%>
(<%= it.backlink %>)
<%- } %>

<%= it.imgEmbed %><%= it.text.replace(/[\r\n]+/g, "\n\n") %>
<% if (it.comment) { %>
> [!note]- 笔记
>
> <%= it.comment.replace(/[\r\n]+/g, "\n>\n> ") %>
<% } %>