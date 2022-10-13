# dynamic-routes-after-deployment

This repo uses default Vue + Vue router template. It has two routes - Home (/)
and About (/about). About route is lazy-loaded. This causes an issue:

- Deploy site
- Open Home route
- Deploy site again (maybe make changes in About route)
- Click on the /about link
- `Failed to fetch dynamically imported module` error will be thrown
