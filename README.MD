Create a new table:
php artisan make:migration create_tableName_table

Add new column:
php artisan make:migration add_columnName_to_tablename_table

Update a column / rename column:
php artisan make:migration update_columnName_to_tablename_table

Remove a column:
php artisan make:migration remove_columnName_from_tablename_table

Drop a table:
php artisan make:migration drop_tableName_table

Patterns for migration names:
const CREATE_PATTERNS = [
    '/^create_(\w+)_table$/',
    '/^create_(\w+)$/',
];
const CHANGE_PATTERNS = [
    '/_(to|from|in)_(\w+)_table$/',
    '/_(to|from|in)_(\w+)$/',
];
