/* Base link style — Nathan's grey, darkening on hover */
a {
    color: $grey-color;
    text-decoration: none;
    font-weight: normal;
    &:hover {
        color: $text-color;
        text-decoration: underline;
    }
}

/* Force sidebar + content links to grey, overriding Bootstrap's blue.
   (The dark navbar's brand/links are more specific, so they stay as-is.) */
.container a,
.col-md-3 a,
.col-md-9 a,
#content a {
    color: $grey-color;
    &:hover { color: $text-color; }
}

/* Footer: grey link that turns white on hover (readable on the dark bar) */
footer a {
    color: $grey-color;
    &:hover { color: #ffffff; }
}
