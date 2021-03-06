# Template Engine

Sebelumnya kita sudah mempelajari bagaimana menerima request dan memberikan respond berupa teks ke client, namun bagaimana apabila kita ingin memberikan respond berupa data yang dimasukkan kedalam html ? caranya adalah menggunakan template engine

![template-engine](template-engine.png)

## Penjelasan Template Engine

**Template Engine** merupakan sebuah tool yang digunakan untuk memasukkan data kedalam sebuah halaman html

## Cara Menggunakan Template Engine Dengan Express

1.  Install template engine yang diinginkan, misalnya pug

    ```
    npm install --save pug
    ```

2.  Mengeset template engine yang akan digunakan, misalnya pug

    ```Javascript
    app.set('views', path.join(__dirname, 'views'))
    app.set('view engine', 'pug')
    ```

3.  Letakkan template di folder views

4.  Untuk merender template, gunakan syntax berikut

    ```Javascript
    res.render('namaTemplate', {data})
    ```

## Beberapa Contoh Template Engine

Berikut contoh - contoh template engine yang dapat digunakan dengan express js :

### 1. Pug

[Dokumentasi](https://pugjs.org/api/getting-started.html)

[Tutorial](https://gist.github.com/joepie91/c0069ab0e0da40cc7b54b8c2203befe1)

[CheatSheet](https://devhints.io/pug)

### 2. EJS

[Dokumentasi](http://ejs.co/#docs)

[Tutorial](https://scotch.io/tutorials/use-ejs-to-template-your-node-application)
