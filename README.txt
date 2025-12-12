# Supabase Auth – Custom Confirmation Email Demo

This is a minimal demo showing how to customize the **Confirm Signup** email sent by
[Supabase Auth](https://supabase.com/docs/guides/auth)
using a fully branded HTML template.

It includes:

- `index.html` – a simple, styled signup UI that triggers the confirmation email
- `email-template.html` – a custom HTML email template you paste into Supabase
- Before/after screenshots to show the difference

This demo is intentionally small and easy to follow: no build tools, no framework, just HTML and Supabase.

---

## 🚀 Try the Demo Locally

1. Clone this repo  
2. Open `index.html` in any browser (no server required)  
3. Enter your email + password  
4. Check your inbox for the Supabase confirmation email

> This demo uses a test Supabase project.  
You can replace the `SUPABASE_URL` and `SUPABASE_ANON_KEY` in `index.html` with your own project.

---

## 🧩 How to Customize the Email Template

Supabase lets you override all Auth email templates.

To use the provided template:

1. Go to **Authentication → Emails → Templates**  
2. Select **Confirm Signup**  
3. Click **</> Source editor**  
4. Paste the content from `email-template.html`  
5. Keep the placeholder:

```html
{{ .ConfirmationURL }}
