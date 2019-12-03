# Stelly's Gatsby + Sanity Starter

---

This is a simple starter repo for bootstrapping Gatsby and Sanity.io projects

## Getting Started:

1. `git clone https://github.com/stelly-dev/starter-gatsby-sanity.git`
2. `cd starter-gatsby-sanity/studio`
3. `sanity init`
4. select `Create new Project`
5. select `Clean Project with no predefined Schemas`
6. Go to sanity.io and create a new token.
7. edit `starter-gatsby-sanity/web/.env-example` and fill out the fields
8. start adding schemas in `starter-gatsby-sanity/studio/schemas/`
9. ???
10. PROFIT

### Wait I forgot how to schema!

No worries, I gotchu. -- here's a quick example.

```js
// blogPost.js
export default {
  name: 'blogPost',
  title: 'Blog Post',
  type: 'document',
  fields: [
    {
      name: 'author',
      title: 'Author',
      type: 'string',
    },

    // ... now you try! ...
  ],
};
```

then import them into `starter-gatsby-sanity/studio/schemas/schema.js`
(don't forget to add to the `schemaTypes.concat([...])` export.

---
