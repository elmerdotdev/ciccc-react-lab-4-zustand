# React JS - Lab Day 4

**Goal:** Create a multi-page CRUD application with React and Zustand. This is similar to the previous lab exercise but with a different state management library and extra features.

## Instructions ✅

1. Create a new React project by running `npm create vite@latest lab-4-crud-zustand`.
2. Create at least seven routes for your application with `react-router-dom`:

    - Home `/`
    - Post Listing `/posts` (only non-deleted items)
    - Post Detail `/posts/1` (where 1 is the id)
    - Add Post `/posts/new`
    - Edit Post `/posts/1/edit` (where 1 is the id)
    - Deleted `/trash` (only deleted items will show up)

3. Implement CRUD functionality for the blog. Store the data and CRUD functions inside a Zustand store like `post.store.ts`. Use Zustand's `persist()` function to keep the data in `localStorage`. For the properties, set them to:

    - id `string` (uuid)
    - title `string`
    - content `string`
    - isDeleted `boolean`

4. Add a **Create** button to the post listing page which redirects you to the *Add Post* route.
5. Add an **Edit** button inside the post detail page which redirects you to the *Edit Post* route to modify the title and content.
6. Add a **Delete** button inside the post detail page which will update the `isDeleted` property to `true`. You can install a toast package such as `react-hot-toast` for the deletion notification. The deleted article will go into the `/trash` page.
7. On the trash listing page, add a **Recover** button beside each post which will update the `isDeleted` property to `false`.
8. On the same trash listing page, add another button called **Delete permanently** which will remove the post from the Zustand store.
9. Commit and push your changes once you are done.

Good luck! 🎉🎉🎉
