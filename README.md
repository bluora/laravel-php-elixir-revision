```
__________.__          ___________.__  .__       .__        
\______   \  |__ ______\_   _____/|  | |__|__  __|__|______ 
 |     ___/  |  \\____ \|    __)_ |  | |  \  \/  /  \_  __ \
 |    |   |   Y  \  |_> >        \|  |_|  |>    <|  ||  | \/
 |____|   |___|  /   __/_______  /|____/__/__/\_ \__||__|   
               \/|__|          \/               \/          
                                             Revision Module
```

Provides the ability to revision specified folders and generate a manifest.

### Revision

Provides revisioning of files in a specified folder location.

Options that are available:

* hash_length - defaults is 8.
* minify - default is false.
* php_manifest - generates a php equivalent of the json revision file.

```
{SOURCE_FOLDER}:
    - {DESTINATION_FOLDER}
    - {REVISION_MANIFEST_FILE}
    - {QUERY_STRING_OPTIONS}
```

```yaml
revision:
    PATH_PUBLIC_ASSETS:
        - PATH_PUBLIC_BUILD
        - PATH_PUBLIC_BUILD + /rev-manifest.json
        - hash_length=12&minify=true&php_manifest=true
```
