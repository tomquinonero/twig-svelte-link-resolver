# Twig Svelte link resolver

This extension allows you to quickly open your svelte components in twig by clicking the links generated in your editor.

<br>
<br>

## Configuration

Prepend the keys with the extension name : **twigSvelteLinkResolver** (e.g. `twigSvelteLinkResolver.templatesRootPath`)

<br>
<table>
    <thead>
        <tr>
            <th>
                Key
            </th>
            <th>
                Description
            </th>
            <th>
                Default
            </th>
            <th>
                Possible values
            </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <span style="text-decoration-line: line-through">templatesRootPath</span>
                <br>
                <b>deprecated, please move your root path to loaderPaths</b>
            </td>
            <td style="text-decoration-line: line-through">
                The relative path to your twig templates folder
            </td>
            <td style="text-decoration-line: line-through">
                "."
            </td>
            <td style="text-decoration-line: line-through">
                any
            </td>
        </tr>
        <tr>
            <td>
                <b>languageFilter</b>
            </td>
            <td>
                What languages are supported for the generated links
            </td>
            <td>
                <pre>
[
    "twig"
]
</pre>
                <i>To enable the generation in twig files you must enable the filters "html" and "twig"</i>
            </td>
            <td>
                All existing language ids supported by Vscode
            </td>
        </tr>
        <tr>
            <td>
                <b>loaderPaths</b>
            </td>
            <td>
                Allows you to specify multiple paths to your twig templates. Add an alias (eg. @App) bounded to a path (eg. src/AppBundle/Resources/views)
            </td>
            <td>
                <pre>
{
    "": ".",
}</pre>
            </td>
            <td>
                alias => string<br>
                path: string (omit the final slash)
            </td>
        </tr>
    </tbody>
</table>

<br>
<br>
