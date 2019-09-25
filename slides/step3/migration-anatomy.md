## Anatomy of a migration

```php
<?php

namespace Migration;

use WP\Migration\MigrationInterface;

class Migration201909221755 implements MigrationInterface
{
    public function execute()
    {
        // ...
    }
}
```
