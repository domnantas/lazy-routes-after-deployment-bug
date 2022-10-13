# dynamic-routes-after-deployment

This repo uses default Vue + Vue router template. It has two routes - Home (/)
and About (/about). About route is lazy-loaded. This causes an issue:

- Deploy site
- Open Home route
- Make changes to About.vue
- Deploy site again
- Click on the /about link
- `Failed to fetch dynamically imported module` error will be thrown
