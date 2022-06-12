# React PWA
Kerangka untuk project create-react-app dengan PWA

## Clone Repository
```bash
git clone https://github.com/saiful-akbar/react-pwa.git
```
## Instal Project Baru

```bash
# Javascript
npx create-react-app project-name --template cra-template-pwa

# Typescript
npx create-react-app my-app --template cra-template-pwa-typescript
```

## Script file `.htaccess` untuk deploy ke cpanel
```batch
<ifModule mod_rewrite.c>

  RewriteEngine On
  RewriteBase /
  RewriteRule ^index.html$ - [L]
  RewriteCond %{REQUEST_FILENAME} !-f
  RewriteCond %{REQUEST_FILENAME} !-d
  RewriteCond %{REQUEST_FILENAME} !-l
  RewriteRule . /index.html [L]

</ifModule>
```
