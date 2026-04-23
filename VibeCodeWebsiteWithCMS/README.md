# Vibe Code a Website with CMS

## Stitch Prompt

Can you design a modern single web page with different sections and top navigation for a dentist office called Waverly Dental Clinic. They already have a logo which is uploaded. Use this logo and match the colour scheme to the logo. Keep the design modern, sleek but welcoming.

## Antigravity Prompt (See note)

### Note

In the prompt below, please replace "**YOUR_WEB_DATA_FORMS_URL**" and "**YOUR_WEB_DATA_FORMS_API_KEY**” with appropriate values from your Web Data Forms account.

### Prompt

Folder “designSource” contains design and HTML for a single web page. Use this to create a nextjs based SSR website. The website should be optimized for performance and SEO, utilizing techniques like code splitting and lazy loading. Use the latest supported version for all packages.

Keep in mind that some of the data on this page will come from a CMS, a single API call - see API endpoint details below. Query this endpoint to find out which data is coming in from this endpoint. For the rest of the data create a JSON object for easy editing later.

API Endpoint: **YOUR_WEB_DATA_FORMS_URL**

The API endpoint REQUIRES BOTH these headers:

“Authorization”: “none”,

“x-wdf-api-key”: “**YOUR_WEB_DATA_FORMS_API_KEY**”

Save the API key above in a env file.

We need a toggle configuration in an env file. When CACHE is set to true always use Incremental Static Regeneration (ISR) strategy to fetch api data. When CACHE is set to false each page refresh should fetch new data from the API.

The site will be deployed on Vercel. So keep in mind that this is a SSR website which fetches and caches data on the server side. Add all Vercel specific packages that are required to deploy this on Vercel.

Provide a running website which fetches date from the API endpoint, caches data or refreshes data based on the CACHE flag and for caching uses Incremental Static Regeneration (ISR) strategy. Keep all image paths relative. Provide a README file with full and detailed instructions on how to run in dev mode, build, the fastest/easiest way to check this project into a Github repository and detail all steps on how to deploy to Vercel.
If you have any questions, please ask me.
