
**General Notes**

**Tailwind CSS**

Tailwind is installed locally with npm. From the project root, run:

```powershell
npm ci
npm run build:css
```

While editing templates, run `npm run watch:css` in a separate terminal alongside
the Django development server. The generated stylesheet is stored in
`onlinecourse/static/onlinecourse/css/tailwind.css` and loaded by all five app
templates. Run `npm run build:css` before deploying or running `collectstatic`.

Use prefixed utilities such as `class="tw:flex tw:gap-4 tw:p-4"`. Tailwind scans
`onlinecourse/templates` for complete class names. Its CSS reset (Preflight) is
disabled and utilities use the `tw:` prefix to preserve the existing Bootstrap
styling. See the [Tailwind Preflight documentation](https://tailwindcss.com/docs/preflight#disabling-preflight).

An `onlinecourse` app has already been provided in this repo upon which you will be adding a new assesement feature.

- If you want to develop the final project on Theia hosted by [IBM Developer Skills Network](https://labs.cognitiveclass.ai/), you will need to create the same project structure on Theia workspace and save it everytime you close the browser
- Or you could develop the final project locally by setting up your own Python runtime and IDE
- Hints for the final project are left on source code files
- You may choose any cloud platform for deployment (default is IBM Cloud Foundry)
- Depends on your deployment, you may choose any SQL database Django supported such as SQLite3, PostgreSQL, and MySQL (default is SQLite3)

**ER Diagram**
For your reference, we have prepared the ER diagram design for the new assesement feature.

![Onlinecourse ER Diagram](https://github.com/ibm-developer-skills-network/final-cloud-app-with-database/blob/master/static/media/course_images/onlinecourse_app_er.png)
