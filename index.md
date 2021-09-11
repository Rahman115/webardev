## Welcome to GitHub

Situs ini akan memberikan pemahaman terkait GitHub.

### A. Melakukan Clone

Perintah 
```markdown
git clone [link-url]
```

### B. Authenticating with Github using an access token
authenticating diperlukan untuk mengirim code program dari PC local ke GitHub Cloud. Sebelum melakukan `git push` baiknya melakukan authenticating terlebih dahulu. Berikut langkah - langkah untuk melakukan authenticating :
1. Membuat Access Token ke GitHub
2. Konfigurasi Repo

Setelah membuat Token, silahkan Copy Token tersebut untuk melakukan konfigurasi. Buka **Terminal** (_Linux_) atau **CMD** (_windows_) untuk melakukan configurasi dan ikuti langkah - lankah berikut ini :
  - Membuka file `~/.bashrc` untuk menyimpan token, gunakan perintah `nano ~/.bashrc` dan __Enter__
  - Tambahkan code berikut ini 
    ```
    GITHUB_ACCESS_TOKEN=pasteyourtokenhere
    ```
  - Kemudian, lakukan pengecekan token yang telah tersimpan, dengan menggunakan perintah `source ~/.bashrc` dan __Enter__ , selanjutnya `echo $GITHUB_ACCESS_TOKEN` dan __enter__ 
  - Setelah muncul token yang telah di paste, Yang dilakukan senjutnya adalah memasukkan code token kedalam `git remote`. Lakukan pengecekan yang akan di**Remote** terlebih dahulu, gunakan perintah `git remote show origin` akan muncul hasil
    ```
    * remote origin
      Fetch URL: https://[your_username]:[your_token]@github.com/[your_name]/[your_repository].git
      Push  URL: https://[your_username]:[your_token]@github.com/[your_name]/[your_repository].git
      HEAD branch: master
      Remote branch:
        master new (next fetch will store in remotes/origin)
      Local ref configured for 'git push':
        master pushes to master (fast-forwardable)
    ```
  - ll

3. Lakukan `git push --set-upstream origin master`




You can use the [editor on GitHub](https://github.com/Rahman115/webardev/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.


Kita akan mencoba beberapa hal di sini

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Rahman115/webardev/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
