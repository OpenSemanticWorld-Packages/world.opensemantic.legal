# world.opensemantic.legal
Privacy policy, Data Protection Information, etc.

The main branch of this repo is a template package.
Please create your own fork and replace [/core/Project/Privacy_policy.wikitext](/core/Project/Privacy_policy.wikitext) with a template-call:

```wikitext
{{Helper/Project/Privacy_policy
|contact=<your data protection office>
|email=<your data protection officer email>
}}
```

`contact` is address of the responsible organization.
If no `email` address is provided, reference is made to the postal `contact` address.

In your forks packages.json, make sure to change `baseURL` to `"https://raw.githubusercontent.com/<your org>/world.opensemantic.meta.legal/<your branch>/core/"`

In case you don't want to maintain your own fork, install the custom branch by adding 
```
https://raw.githubusercontent.com/OpenSemanticWorld-Packages/world.opensemantic.meta.legal/custom/packages.json
```
to your package index or by adding
```
$wgPageExchangePackageFiles[] = 'https://raw.githubusercontent.com/OpenSemanticWorld-Packages/world.opensemantic.meta.legal/custom/packages.json';
```
to `mediawiki/config/CustomSettings.php` of your OSL instance. After doing so, you can edit the page `Project:Privacy_policy` manually to include the template showed above.

