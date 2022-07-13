# Laravel Multi layout Issue

We Identify that when we have multi type of layouts like `user/merchant/simple-uer/seller` which have common interface but different navigations and assets files than we have to create multiple `app.blade.php` in every layout type to load navigation/section or asset files.

## We Resolved

So we make some files which will help you to load multiple sections & assets file in one main layout file named `main.blade.php` which is depend on `Helper` file and two files `load_top.blade.php` & `load_bottom.blade.php` which will load sections around `@yeild('content')`
