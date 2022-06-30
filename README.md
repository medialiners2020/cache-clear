# cache-clear
__Incluir código no final do arquivo de routes\web.php__
```php
Route::get('/clear-cache', function() {
    Artisan::call('cache:clear');
    Artisan::call('config:clear');
    Artisan::call('view:clear');
    return redirect('/');
});

```
__Para executar, basta realizar a chamada pela rota criada /clear-cache__
