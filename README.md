# svg-render-assets

Static SVG test assets used to demonstrate how a document-context SVG renderer
reports its own execution origin.

`poc.svg` contains a small inline script. The script makes no network request,
reads no credential, writes to no storage, and touches nothing outside the
document it is loaded into. It prints `document.domain`, `window.origin`,
`document.contentType` and the root element name into the image itself.

These files support an authorized, privately reported vulnerability disclosure
and are not an attack against any third party.
