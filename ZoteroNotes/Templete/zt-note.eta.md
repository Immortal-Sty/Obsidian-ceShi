
# <%= it.title ?? it.DOI ?? it.citekey ?? it.key %>
<% if(it.abstractNote) { -%>

> [!note] <%= it.abstractNote.first().replace(/[\r\n]+/g, "\n>\n> ") %>

<% } -%>
[Zotero](<%= it.backlink %>) <%= it.fileLink %>
<%~ include("annots", it.annotations) %>