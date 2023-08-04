# Schema

<div id="swagger-ui"></div>
<link rel="stylesheet" type="text/css" href="//unpkg.com/swagger-ui-dist@3/swagger-ui.css" />
<script src="//unpkg.com/swagger-ui-dist@3/swagger-ui-bundle.js"></script>
<script>
var href = window.location.href.toString();
const schema_path = href.replace("html", "yaml")
const ui = SwaggerUIBundle({
    url: schema_path,
    dom_id: '#swagger-ui',
    presets: [
        SwaggerUIBundle.presets.apis,
        SwaggerUIBundle.SwaggerUIStandalonePreset
    ],
    layout: "BaseLayout",
    supportedSubmitMethods: [],
    operationsSorter : "alpha",
    tagsSorter: 'alpha'
    });
</script>