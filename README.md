**Links for helping**

1. https://docs.cypress.io/api/table-of-contents
2. https://example.cypress.io/
3. https://filiphric.com/blog
4. https://glebbahmutov.com/cypress-examples/8.4.0/

**Assertions**
https://www.chaijs.com/api/bdd/#method_oneof

https://docs.cypress.io/guides/references/assertions#BDD-Assertions

https://docs.cypress.io/guides/references/assertions#Chai-jQuery

**Selectors** 
https://api.jquery.com/category/selectors/


# Global problems and solutions
- [Long wait for cypress to download the file](#Long-wait-for-cypress-to-download-the-file)

## Long wait for cypress to download the file

```
    cy.window().document().then(function (doc) {
      doc.addEventListener('click', () => {
        setTimeout(function () { doc.location.reload() }, 5000)
      })
      cy.contains('Download file template').click()
    })
```

> Where `cy.contains('Download file template').click()` you need to change instead your selector
