ANGERMUND TRANSPORT FULL BACKEND NETLIFY SITE

IMPORTANT:
This backend version cannot be uploaded through simple Netlify Drop only.
Use GitHub import or Netlify CLI, because it includes Netlify Functions.

WHAT IS INCLUDED:
- Login system
- Cloud database using Netlify Blobs
- Multi-user roles: admin, manager, driver
- Admin users page
- Editable fleet/trucks
- Trips with rate per KM and profit/loss
- Profit/loss by driver, truck, route
- Fuel, expenses, permits, invoices, workers
- GPS location capture from driver phone
- WhatsApp report generator
- Invoice print/PDF screen
- PWA install to Android home screen

DEMO LOGIN:
admin / admin123
driver1 / driver123

DEPLOY WITH GITHUB:
1. Upload this whole folder to GitHub.
2. Netlify > Add new site > Import from Git.
3. Select the repo.
4. Build command: npm install
5. Publish directory: public
6. Functions directory: netlify/functions
7. Add environment variable:
   JWT_SECRET = any long private random text
8. Deploy.

LOCAL TEST:
1. Install Node.js
2. npm install
3. npx netlify dev

NOTES:
- WhatsApp uses click-to-send link. Real automated WhatsApp messages need WhatsApp Business Cloud API.
- GPS captures driver phone location when driver presses the location button. Continuous live tracking needs a mobile background app.
- Invoice PDF uses browser print/save as PDF.
