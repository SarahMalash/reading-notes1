# read 12:
## when dose Partials come in handy?
when you want to reuse the same HTML across multiple views
*makes large websites easier to maintain as you don’t have to go and change a piece of text in every page it appears in*

*any JavaScript or non-HTML syntax you include in your templates is always surrounded by <% %> delimiters*
 ## Including a partial in EJS:
  You use <%- include( PARTIAL_FILE ) %>

  *The <%- %> tags allow us to output the unescaped content onto the page (notice the -)*
  