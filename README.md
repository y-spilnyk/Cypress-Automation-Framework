# Links for helping

1. https://docs.cypress.io/api/table-of-contents
2. https://example.cypress.io/
3. https://filiphric.com/blog
4. https://glebbahmutov.com/cypress-examples/8.4.0/


#Global problems and solutions

    ```cy.window().document().then(function (doc) {
      doc.addEventListener('click', () => {
        setTimeout(function () { doc.location.reload() }, 5000)
      })
      cy.contains('Download file template').click()
    })
    ```
