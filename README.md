# Symfony Recipes

This repository contains recipes for Composer packages developed by the [Specter.Global](https://specter.global) Team.

For comprehensive details regarding the recipes and their usage, please refer to the
Specter.Global [Symfony recipes documentation](https://developer.specter.global/docs/symfony-recipes).

## Configure Access to Recipes

Update `composer.json` file with an extra Symfony Flex endpoint to allow the execution of the recipes.

Execute the following command:

```shell
composer config extra.symfony.endpoint \
    '["https://api.github.com/repos/specter-global/app-tmp-recipes/contents/index.json?ref=flex/main", "flex://defaults"]' \
    --json \
    --merge
```

The updated `composer.json` file should now have the following contents:

```json
{
    "extra": {
        "symfony": {
            "endpoint": [
                "https://api.github.com/repos/specter-global/app-tmp-recipes/contents/index.json?ref=flex/main",
                "flex://defaults"
            ]
        }
    }
}
```

<div style="text-align: center">
    <a href="https://developer.specter.global/docs/symfony-recipes" target="_blank">
        <picture>
            <source media="(prefers-color-scheme: dark)" srcset="https://specter.global/favicon-32x32.png">
            <source media="(prefers-color-scheme: light)" srcset="https://specter.global/favicon-32x32.png">
            <img alt="Specter.Global" src="https://specter.global/favicon-32x32.png">
        </picture>
    </a>
</div>
