### How to hide `Powered by the Academic theme for Hugo` from the footer of Hugo Academic theme.
- Inside config/_default/config.yml file, change all module import paths to respective ones starting with `Saydemr`. \
    e.g.
    ```
    module:
      imports:
        - path: github.com/Saydemr/wowchemy-hugo-themes/modules/wowchemy-plugin-netlify-cms
        - path: github.com/Saydemr/wowchemy-hugo-themes/modules/wowchemy-plugin-netlify
        - path: github.com/Saydemr/wowchemy-hugo-themes/modules/wowchemy-plugin-reveal
        - path: github.com/Saydemr/wowchemy-hugo-themes/modules/wowchemy
    ```
- Inside go.mod file, change the require statements as follows
  ```
  require (
    github.com/Saydemr/wowchemy-hugo-themes/modules/wowchemy-plugin-netlify v0.0.0-20220924111144-7d5796d8f96a
    github.com/Saydemr/wowchemy-hugo-themes/modules/wowchemy-plugin-netlify-cms v0.0.0-20220924111144-7d5796d8f96a
    github.com/Saydemr/wowchemy-hugo-themes/modules/wowchemy v0.0.0-20220924111144-7d5796d8f96a
  )
  ```
