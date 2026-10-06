# Select Game Store

Pre-owned PS4 / PS5 game store website (Port Said, Egypt). Single static file, no build step.
موقع متجر Select Game Store لبيع ألعاب بلايستيشن 4 و 5 المستعملة. ملف واحد بدون أي تثبيت.

## Put it online with GitHub Pages | النشر على GitHub Pages

1. Create a new repository on github.com (for example `select-store`), public.
2. Upload **all files in this folder** (`index.html`, `.nojekyll`, `README.md`) to the repository root.
3. Go to **Settings > Pages**. Under *Build and deployment* choose **Deploy from a branch**, branch `main`, folder `/ (root)`, then Save.
4. After about a minute your site is live at `https://YOUR-USERNAME.github.io/select-store/`.

بالعربي: اعمل Repository جديد على GitHub، ارفع الملفات كلها، ثم من Settings > Pages اختار Branch `main` و Folder `/ (root)` واضغط Save. الموقع يشتغل بعد دقيقة تقريباً.

## Managing the store (admin) | إدارة المتجر

- Open the site, pick a language, then **Log in** with the admin email and password. Anyone else who signs up or logs in is a normal customer.
- You can edit prices, stock, photos, YouTube links, categories, main categories, store settings and add new games.
- **One-time setup (2 minutes):** in the admin bar press **Live setup** and enter your GitHub username, repository name and an access token (the page explains how to create it: a *fine-grained token* limited to this one repository with *Contents: Read and write*). Press **Test connection**, then **Save**.
- After that, press **Publish changes** whenever you edit. The site sends your changes straight to GitHub and customers see them in about a minute. You never upload files again.
- The token is stored only in your own browser. If you use another phone or computer, enter it there once.
- Photos are saved as separate files in the `img/` folder and the data in `store-data.json`. Do not delete them.

بالعربي: اضغط Live setup مرة واحدة وحط اسم حسابك على GitHub واسم المستودع و Token (الصفحة بتشرح ازاي تعمله). بعدها كل ما تعدل اضغط Publish changes والتعديلات بتظهر للعملاء بعد حوالي دقيقة بدون ما ترفع أي ملف.

## Good to know | ملاحظات

- Upload the whole folder: `index.html`, `store-data.json`, the `img/` folder, `.nojekyll`.
- The admin password is stored only as a salted hash, never as plain text. A short numeric password can still be guessed by someone determined, but on GitHub that only opens the admin screen in *their own* browser: nobody can change what other visitors see unless they can commit to your repository. Use a long password anyway (Store settings > New admin password) and turn on two-factor authentication on your GitHub account.
- Customer accounts are saved on each customer's own device. They are not shared and you cannot see them.
- The assistant on GitHub answers from built-in PlayStation knowledge and your live stock list. The smarter version only runs inside Claude.
- Customer orders open WhatsApp with the order text. Set the number in Store settings.
- Google Fonts needs internet access. If it is blocked the site falls back to system fonts.
