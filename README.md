/* ----- reset.css ----- */
html, body, div, span, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, code,
del, dfn, em, img, q, dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td {
  margin: 0;
  padding: 0;
  border: 0;
  font-weight: inherit;
  font-style: inherit;
  font-size: 100%;
  font-family: inherit;
  vertical-align: baseline;
}

body {
  line-height: 3.3;
  text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -ms-text-size-adjust: 100%;
  -moz-text-size-adjust: 100%;
  -o-text-size-adjust: 100%;
    background: #202020;
}



table { border-collapse: separate; border-spacing: 0; }
caption, th, td { text-align: left; font-weight: normal; }
table, td, th { vertical-align: middle; }

blockquote:before, blockquote:after, q:before, q:after { content: ""; }
blockquote, q { quotes: "" ""; }

a img { border: none; }

/* ----- Clearfix ----- */
.clearfix:after { content: "."; display: block; clear: both; visibility: hidden; line-height: 0; height: 0; }
.clearfix { display: inline-block; }
html[xmlns] .clearfix { display: block; }
* html .clearfix { height: 1%; }
* { box-sizing: border-box; }
/* ----- Clearfix end ----- */


/* ----- Smooth shaking animation ----- */
.shaking {
    animation: shake .5s linear;
}

@keyframes shake {
    8%, 41% {
        transform: translateX(-10px);
    }
    25%, 58% {
        transform: translateX(10px);
    }
    75% {
        transform: translateX(-5px);
    }
    92% {
        transform: translateX(5px);
    }
    0%, 100% {
        transform: translateX(0);
    }
}
/* ----- Smooth shaking animation end ----- */





/* ----- General layout ----- */
body {
    margin: 0;
    scroll-behavior: smooth;
    overflow-x: hidden;
}
.header .network {
    display: inline-block;
    vertical-align: top;
    position: relative;
}
.header .network:after {
    content: "";
    position: absolute;
    top: 13px;
    right: 9px;
    pointer-events: none;
    width: 0;
    height: 0;
    border-style: solid;
    border-width: 4px 4px 0 4px;
    border-color: grey transparent transparent transparent;
}
.network optgroup {
    font-size: 13px;
    font-family: unset;
    font-weight: bold;
}
.network select:active {
    box-shadow: rgba(0, 0, 0, 0.1) 0px 1px 1px 0px;
}
.network select:hover {
    border: 1px solid #c6c6c6;
    color: #333;
    background-image: linear-gradient(to bottom,#f8f8f8,#f1f1f1);
}
.network select::-ms-expand {
    display: none;
}
.network select {
    background-image: linear-gradient(to bottom,#f8f8f8,#f1f1f1);
    border: 1px solid rgba(0,0,0,0.1);
    color: #444;
    font-size: 11px;
    font-weight: bold;
    text-align: center;
    outline: none;
    white-space: nowrap;
    padding: 8px;
    padding-right: 22px;
    position: relative;
    border-radius: 2px;
    appearance: none;
    -moz-appearance: none;
    -ms-appearance: none;
    -o-appearance: none;
    -webkit-appearance: none;
}
.header {
    user-select: none;
    margin-top: 15px;
    width: 100%;
}
.header .left-side {
    float: left;
}

.header .left-side .logo {
    display: inline-block;
    vertical-align: middle;
}

.header .left-side .fffff {
    top: -4px;
    left: 12px;
    position: relative;
}

.header .left-side img {
    max-height: 35px;
}
.header .right-side {
    float: right;
}
.container {
    width: 70%;
    margin: 0 auto;
}
.content {
    position: relative;
    margin-left: 58px;
    margin-right: 9px;
}
.content .section {
    font-family: "Roboto", sans-serif;
    position: relative;
    margin: 0px 0 0px 0;
}

.content .section > .icon {
    display: inline-block;
    overflow: hidden;
    user-select: none;
    position: absolute;
    width: 45px;
    height: 45px;
    top: 0;
    left: -54px;
    padding-top: 2.5px;
    padding-left: 7.5px;
}

.content .section .body {
    width: 100%;
    position: relative;
    word-break: break-word;
}

.content .section .body-content {
    margin-top: 5px;
}

.content .section .body-content.tos-page p {
    margin-bottom: 10px;
}

.content .section .body-content.tos-page h2 {
    margin-bottom: 5px;
    font-weight: bold;
}

.content .section .secondary {
    color: black;
    font-weight: bold;
    text-transform: lowercase;
    display: inline-block;
    padding-left: 4px;
    margin: 0;
    font-size: 27px;
}

.content .section .secondary, .side label .status.active {
    opacity: 0.35;
}

.content .section .primary {
    position: relative;
    font-size: 27px;
    font-weight: bold;
    text-transform: lowercase;
    margin: 0;
    display: inline-block;
    color: #5581b5;
}

.section.tool-title .body-content a,
.section.front-primary .body-content a {
    color: #5581b5;
}

.section.announcement .primary, .section.announcement .icon {
    color: #e05746;
}

.announcement-new {
    color: #444;
    font-family: "Roboto", sans-serif;
}
.announcement-new-title {
    font-size: 16px;
    font-weight: 500;
}
.announcement-new-title .primary {
    color: #e05745;
}
.announcement-new-title .secondary {
    opacity: 0.75;
}
.announcement-new-body {
    font-size: 14px;
    margin-top: 2px;
}
/* ----- General layout end ----- */

/* ----- Old browser warning ----- */

.content .section.old-browser .primary, .content .section.old-browser .icon {
    color: #e05746;
}

.content .section.old-browser .tool-message {
    padding-top: 5px;
    color: #e05746;
}

/* ----- Old browser warning end ----- */



/* ----- Converter styling ----- */
.sides-primary-button {
    margin-top: 15px;
}
.sides-primary-button button:active {
    box-shadow: 0 1px 0 0 #2e4765;
    transform: translateY(2px);
}
.sides-primary-button button {
    position: relative;
    transition: all 0.1s ease;
    width: 100%;
    border: none;
    outline: none;
    font-family: "Roboto";
    text-shadow: 0px 1px 0px black;
    font-weight: bold;
    color: white;
    font-size: 18px;
    padding: 10px 0 10px 0;
    box-shadow: 0px 3px 0 0 #2e4765;
    background: #476c98;
    border-radius: 5px;
    cursor: pointer;
}

/* Sublime Monokai default editor theme */
.side[data-theme="theme-editor"] label {
    color: #7b756a;
}
.side[data-theme="theme-editor"] .side-wrapper {
    background: #7b756a;
}
.sides .side[data-theme="theme-editor"] .side-wrapper:after {
    border-bottom: 8px #7b756a solid;
}
.side[data-theme="theme-editor"] .side-widgets {
    background: #7b756a;
    box-shadow: inset 0px 6px 6px -6px rgba(0, 0, 0, 0.5), 0px 3px 0 0 black;
}

/* Plaintext editor theme */
.side[data-theme="theme-plain"] label {
    color: #476c98;
}
.side[data-theme="theme-plain"] .side-wrapper {
    background: #f7f7f7;
}
.sides .side[data-theme="theme-plain"] .side-wrapper:after {
    border-bottom: 8px #f7f7f7 solid;
}
.side[data-theme="theme-plain"] .side-widgets {
    background: #ececec;
    box-shadow: inset 0px 6px 6px -6px rgba(0, 0, 0, 0.5), 0px 3px 0 0 #cccccc;
}
.side[data-theme="theme-plain"] .side-widgets .widget {
    color: #505050;
    text-shadow: none;
}

/* Binary editor theme */
.side[data-theme="binary"] label {
    color: black;
}
.side[data-theme="binary"] .side-wrapper {
    background: black;
    padding: 0;
}
.sides .side[data-theme="binary"] .side-wrapper:after {
    border-bottom: 8px black solid;
}
.sides .side[data-theme="binary"] .data-wrapper {
    height: 306px;
}
.side[data-theme="binary"] .side-widgets {
    background: #2f2f2f;
    box-shadow: inset 0px 6px 6px -6px rgba(0, 0, 0, 0.5), 0px 3px 0 0 black;
}
.side[data-theme="binary"] .side-widgets .widget {
    color: white;
    text-shadow: none;
}

.side[data-theme="binary"] .tool-combinator {
    background: #2f2f2f;
    box-shadow: 0 -3px #1a1a1a;
}
.sides .side[data-theme="binary"].error .side-wrapper {
    background: black;
}

.side {
    width: 48%;
    top: 0;
    font-size: 0;
    transition: width 0.2s ease;
    position: relative;
    display: inline-block;
    font-family: monospace;
}
.side:only-child {
    width: 100%;
}
.side > label {
    transition: left 0.2s ease;
}
.side > label .status {
    color: black;
    opacity: 0;
    transition: opacity 0.2s ease;
}
.sides-wrapper {
    width: 100%;
}
.sides-options-wrapper {
    margin-top: -10px;
}
.side > label, .sides-options-wrapper > label.caption {
    letter-spacing: -1px;
    text-transform: lowercase;
    user-select: none;
    position: relative;
    width: 100%;
    top: 0;
    margin-bottom: 5px;
    display: inline-block;
    font-size: 0px;
    left: 0;
    font-weight: bold;
    font-family: "Roboto";
    color: #7a7262;
}

.sides {
    width: 100%;
    padding-top: 7px;
}
.sides-wrapper.muted {
    opacity: 0.75;
}
.sides .side.error .side-wrapper:after {
    border-bottom: 8px rgba(85, 129, 181, 0.75) solid;
}
.sides .side .side-wrapper:after, .onlinetools-subscribe-box:before, .converter-options:before, .feedback-box:before, .tool-none-matches .message:before {
    content: '';
    position: absolute;
    width: 0;
    height: 0;
    top: -16px;
    border-top: 8px transparent solid;
    border-left: 8px transparent solid;
    border-right: 8px transparent solid;
    border-bottom: 0px #7a7262 solid;
    left: 24px;
    transform: translateX(-10px);
}

.sides .side-widgets {
    position: relative;
    overflow: hidden;
    user-select: none;
    font-family: "Roboto";
    font-size: 0;
    box-shadow: inset 0px 6px 6px -6px rgba(0, 0, 0, 0.5), 0px 3px 0 0 #171717;
    background: #303134;
    border-radius: 0 0 5px 5px;
}
.side-widgets .widget {
    display: inline-block;
    position: relative;
    cursor: pointer;
    padding: 10px;
    font-size: 30px;
	left:10px;
    text-align: center;
    color: white;
    width: 33.333%;
    vertical-align: center;
    font-weight: bold;
    text-shadow: 0px 1px 0px black;
}
.widget.widget-remove-chain-wrap {
    position: relative;
    width: 100%;
}
.toggle-remove-chain .remove-chain-text {
    position: absolute;
    left: 20px;
    text-align: left;
    top: -1px;
    opacity: 0.5;
    bottom: 0;
    right: 0;
    display: block;
}
.toggle-remove-chain .remove-chain-yes {
    position: absolute;
    right: 6px;
    top: -3px;
    bottom: 0;
}
.toggle-remove-chain .remove-chain-yes .svg-icon {
    fill: white;
    width: 24px;
    height: 24px;
}
.sides.tool .side.output .side-widgets .widget-remove-chain, .sides.tool.is-chained .side.output .side-widgets .widget-chain {
    display: none;
}
.sides.tool.is-chained .side.output .side-widgets .widget-remove-chain, .sides.tool .side.output .side-widgets .widget-chain {
    display: inline-block;
}
.widget-toggle .widget-chain-search {
    cursor: default;
    width: 100%
}

.widget-chain-search .chain-search-wrapper {
    left: 44px;
    top: -1px;
    right: 0;
    position: absolute;
    height: 100%;
}
.widget-chain-search .svg-icon {
    display: none;
    position: absolute;
    opacity: 0.5;
    left: 12px;
    top: -1px;
    width: 24px;
    height: 24px;
    fill: white;
}
.widget-toggle .widget-chain-search.state-wait .icon_wait {
    display: block;
}
.widget-toggle .widget-chain-search.state-search .icon_search {
    display: block;
}
.widget-toggle .widget-chain-search.state-error .icon_error {
    display: block;
}
.widget-chain-search .chain-search::placeholder {
    color: rgba(255, 255, 255, 0.5);
}
.tool-combinator {
    position: absolute;
    overflow: hidden;
    font-family: "Roboto";
    z-index: 99;
    background: #41628b;
    border-radius: 5px 5px 0 0;
    box-shadow: 0 -3px hsla(213, 36%, 33%, 1);
    right: 0;
    left: 0;
    bottom: 0;
    height: 0;
    transition: all 0.5s ease;
}
.side.output.combinator-active .tool-combinator {
    height: 175px;
}
.combinator-description {
    display: block;
    font-size: 13px;
    color: rgba(255, 255, 255, 0.75);
}
.combinator-title {
    font-size: 15px;
    vertical-align: middle;
    line-height: 19px;
    display: inline-block;
    text-shadow: 0px 1px rgba(0, 0, 0, 0.5);
}
.combinator-tool {
    width: 50%;
    cursor: pointer;
    padding: 0px 4px 4px 8px;
    display: inline-block;
    transition: all 0.3s cubic-bezier(.25, .8, .25, 1);
    border-radius: 4px;
    clear: none;
}
.combinator-tool:hover {
    background-color: rgba(255, 255, 255, 0.1);
    box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}
.combinator-tool.hidden {
    opacity: 0.4;
    pointer-events: none;
}
.combinator-tools {
    display: flex;
    flex-wrap: wrap;
}
.combinator-list {
    padding: 0 5px 5px 5px;
    position: absolute;
    right: 4px;
    left: 0;
    top: 3px;
    bottom: 3px;
    overflow-y: auto;
}
.widget-chain-search .chain-search {
    position: absolute;
    left: 0;
    top: 0;
    border: 0;
    width: 100%;
    background: transparent;
    color: white;
    outline: none;
    font-size: 16px;
    font-family: "Roboto";
}
.side-widgets .side-widgets-toggle {
    transform: rotateX(90deg) translateY(-50%) translateZ(22px);
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}
.side-widgets.toggled .side-widgets-wrapper:after {
    background: rgba(0, 0, 0, 0.5);
}
.side-widgets.toggled .side-widgets-toggle:after {
    background: transparent;
}
.side-widgets .side-widgets-wrapper:after, .side-widgets .side-widgets-toggle:after {
    width: 100%;
    height: 100%;
    content: "";
    position: absolute;
    left: 0;
    top: 0;
    pointer-events: none;
    background: transparent;
    transition: background 0.5s ease;
}
.side-widgets .side-widgets-toggle:after {
    background: rgba(0, 0, 0, 0.5);
}

.side-widgets.toggled .side-widgets-toggle, .side-widgets .side-widgets-wrapper {
    transform: rotateX(0deg) translateY(0px) translateZ(0px);
}
.side-widgets.toggled .side-widgets-wrapper {
    transform: rotateX(-90deg) translateZ(22px) translateY(50%);
}
.side-widgets-wrapper, .side-widgets-toggle {
    transition: transform 0.5s ease;
}

.side-widgets-toggle .toggle-wrapper {
    position: relative;
    top: 50%;
    transform: translateY(-50%);
}

.side-widgets-toggle .widget-toggle {
    margin-right: 44px;
    display: none;
}
.side-widgets-toggle .widget-toggle.toggle-active {
    display: block;
}
.side-widgets-toggle .toggle-save-as .widget {
    width: 50%;
}
.side-widgets-toggle .toggle-unchainable .widget {
    width: 100%;
    opacity: 0.5;
    text-align: center;
    cursor: default;
}
.toggle-hide {
    position: absolute;
    cursor: pointer;
    right: 0;
    top: 0;
    height: 100%;
    width: 44px;
    text-align: center;
}
.toggle-hide .svg-icon {
    fill: white;
    top: 50%;
    transform: translateY(-50%);
    position: relative;
    text-shadow: 0px 1px 0px black;
    width: 24px;
    height: 24px;
}
.side-widgets .widget.is-inactive {
    opacity: 0.5;
}
.side-widgets .widget.is-disabled {
    opacity: 0.5;
    cursor: default;
    pointer-events: none;
}
.widget-load input {
    display: none;
}
.sides .side.error .side-widgets {
    opacity: 0.75;
}
.sides .side.error .side-wrapper {
    background: rgba(85, 129, 181, 0.75);
    box-shadow: none;
}
.sides .side.error .data-type{
    color: rgba(85, 129, 181, 0.75);
    position: relative;
}
.side.error label .data-type:before {
    position: absolute;
    content: "";
    left: 0;
    top: 50%;
    right: 0;
    border-radius: 5px;
    border-top: 4px red solid;
    transform: rotate(-10deg);
}
.sides .side.input {
    float: left;
}
.sides .side.output {
    float: right;
}
.sides.section > .icon {
    top: 8px;
}

.sides.expanded .side {
    width: 100%;
}
.sides.expanded .side.output {
    float: left;
    margin-top: 20px;
}
.tool-inline {
    position: absolute;
    left: -44px;
    top: 60px;
}
.tool-inline .svg-icon {
    fill: rgba(0, 0, 0, 0.25);
    transition: color 0.1s ease;
    user-select: none;
    width: 29px;
    height: 29px;
}
.tool-toggle-layout svg.expand, .sides.expanded .tool-toggle-layout svg.expanded {
    display: block;
}
.tool-toggle-layout svg.expanded, .sides.expanded .tool-toggle-layout svg.expand {
    display: none;
}

.tool:nth-child(odd) .chain-link {
    right: -75px;
    position: absolute;
    display: block;
    top: 235px;
    border: 5px #d1d1d1 dashed;
    border-left: none;
    width: 25px;
    border-radius: 0 5px 5px 0;
    height: auto;
    bottom: -225px;
}
.tool:nth-child(even) .chain-link {
    position: absolute;
    display: block;
    left: -75px;
    top: 235px;
    border: 5px #d1d1d1 dashed;
    border-right: none;
    width: 25px;
    border-radius: 5px 0 0 5px;
    height: auto;
    bottom: -225px;
}

.tool + .tool:before {
    content: "settings";
    position: absolute;
    display: inline-block;
    white-space: nowrap;
    left: -46px;
    top: -2px;
    visibility: hidden;
    font-family: "Material Icons";
    color: rgba(0, 0, 0, 0.35);
    font-size: 35px;
}

.tool:nth-child(odd) .chain-link:after {
    content: "";
    bottom: -8px;
    display: block;
    position: absolute;
    left: -10px;
    width: 0;
    height: 0;
    border-bottom: 6px solid transparent;
    border-top: 6px solid transparent;
    border-right: 10px solid #d1d1d1; 
    font-size: 0;
    line-height: 0;
}

.tool:nth-child(even) .chain-link:after {
    content: "";
    bottom: -8px;
    display: block;
    position: absolute;
    right: -10px;
    width: 0;
    height: 0;
    border-bottom: 6px solid transparent;
    border-top: 6px solid transparent;
    border-left: 10px solid #d1d1d1;
    font-size: 0;
    line-height: 0;
}
.tool:last-child .chain-link {
    display: none;
}
.tool-primary {
    margin-bottom: 0;
}
.tool-primary:last-child {
    margin-bottom: 30px;
}
.tool-chained {
    margin: 0;
}
.tool-chained .icon_settings, .tool-chained .tool-inline {
    display: none;
}



.tool-toggle-layout:hover .svg-icon,
.tool-swap:hover .svg-icon,
.tool-favorite:hover .svg-icon,
.tool-create-link:hover .svg-icon,
.tool-create-link.active .svg-icon,
.tool-tweet:hover .svg-icon
{
    fill: rgba(0, 0, 0, 0.4);
}
.tool-tweet a {
    position: absolute;
    width: 100%;
    height: 100%;
}
.tool-toggle-layout, .tool-swap, .tool-favorite, .tool-create-link, .tool-tweet {
    cursor: pointer;
    position: relative;
    width: 29px;
    height: 29px;
    margin-bottom: 5px;
}
.tool-create-link.active .tool-link {
    opacity: 1;
    visibility: visible;
    bottom: -90px;
    padding: 5px 10px 10px;
}
.tool-link input[type="text"] {
    width: 100%;
    display: block;
    padding: 4px;
    outline: none;
    border: none;
    background: rgba(0, 0, 0, 0.15);
    color: white;
    border-radius: 3px;
    box-shadow: inset 0 0 3px 0 rgba(0, 0, 0, 0.75), 0 0 0 1px rgba(255, 255, 255, 0.15);
}
.tool-link {
    opacity: 0;
    visibility: hidden;
    transition: all 0.2s ease;
    bottom: -65px;
    position: absolute;
    font-size: 14px;
    white-space: normal;
    border-radius: 3px;
    color: white;
    min-width: 35px;
    width: 265px;
    left: -1px;
    z-index: 10;
    padding: 5px;
    background: #476c98;
    box-shadow: 0px 3px 0 0 #2e4765, 0 4px 6px rgba(0,0,0,0.16), 0 4px 6px rgba(0,0,0,0.23);
}
.tool-link-text {
    margin-bottom: 5px;
}
.tool-link:before {
    position: absolute;
    left: 9px;
    top: -7px;
    content: "";
    width: 0;
    height: 0;
    border-style: solid;
    border-width: 0 8px 8px 8px;
    border-color: transparent transparent #476c98 transparent;
}
.tool-create-link i {
    font-size: 24px;
    padding-left: 3px;
}
.tool-favorite i {
    font-size: 26px;
    padding-left: 2px;
}
.tool-swap[data-swap-to=""] {
    display: none;
}
.side-wrapper.immersive {
    padding: 0;
}
.side-wrapper.immersive:after {
    display: none;
}
.side-wrapper.horizontal-scrollbar textarea.data {
    white-space: pre;
    overflow-x: auto;
    overflow-y: auto;
}
.side-wrapper {
    z-index: 2;
    user-select: none;
    padding: 3px;
    font-size: 16px;
    position: relative;
    background: #303134;
    color: white;
    border-radius: 5px 5px 0 0;
}
.sides .tool-favorite.active svg {
    fill: #f7d000;
    text-shadow: 0px 1px 1px rgba(0, 0, 0, 0.15);
}
.converter-options .option-group-legend {
	padding-left: 30px;
    font-weight: bold;
    text-shadow: 0px 1px 0px #202020;
    margin-bottom: 0px;
    display: block;
}

.converter-options .option-group input[type="text"]:disabled, .converter-options .option-group textarea:disabled {
    opacity: 0.75;
    cursor: default;
}
.side.input .side-box.empty .input-canvas-help {
    display: block;
}
.input-canvas-help span {
    display: block;
    position: relative;
    top: 50%;
    width: 80%;
    margin: 0 auto;
    transform: translateY(-50%);
    font-family: "Roboto";
    color: rgba(0, 0, 0, 0.5);
    font-size: 18px;
    text-shadow: 0 1px white;
}
.input-canvas-help {
    position: absolute;
    pointer-events: none;
    user-select: none;
    width: 100%;
    height: 100%;
    display: none;
}
.input-canvas-help .help-mouse, .dragging .input-canvas-help .help-normal, .input-canvas-help .help-wait, .importing .input-canvas-help .help-normal {
    display: none;
}
.dragging .input-canvas-help .help-mouse, .importing .input-canvas-help .help-wait {
    display: block;
    text-align: center;
}
.side-box.empty .side-wrapper {
    background: rgba(0, 0, 0, 0.1);
}
.side-box.empty .side-widgets:after {
    display: none;
}
.side-box.empty .side-widgets {
    box-shadow: none;
    border-top: 1px rgba(0, 0, 0, 0.15) dashed;
    padding-bottom: 2px;
    background: rgba(0, 0, 0, 0.1);
}
.side-box.empty .side-widgets .widget, .side-box.empty .side-widgets .toggle-hide .icon {
    color: rgba(0, 0, 0, 0.3);
    text-shadow: 0 1px white;
}
.side-box.empty {
    box-shadow: inset 0 0 10px 0 rgba(0, 0, 0, 0.5);
    border-radius: 5px;
}
.data-wrapper {
    height: 300px;
}
.multitype-input .multitype-mode {
    display: none;
    width: 100%;
    height: 100%;
}
.multitype-input[data-multitype-mode="text"] .mode-text {
    display: block;
}
.multitype-input[data-multitype-mode="file"] .mode-file {
    display: block;
}
.data, .preview {
    resize: none;
	font-size:5px;
    outline: none;
    border: none;
    display: block;
    transition: margin-top 0.1s ease;
    background: transparent;
    color: white;
    height: 100%;
    position: relative;
    width: 100%;
    overflow-x: hidden;
    overflow-y: auto;
    padding-right: 0px;
}
.side.input canvas.preview {
    cursor: pointer;
}
canvas.preview, canvas.data {
    padding: 0;
    height: 306px;
    border-radius: 5px 5px 0 0;
    image-rendering: pixelated;
}
textarea.data {
    font-family: "SFMono-Regular", Consolas, "Liberation Mono", Menlo, Courier, monospace;
}

/* Removes Webkit scrollbars */
.preview-scrollable::-webkit-scrollbar {
    display: none;
}

/* Removes Firefox scrollbars */
.preview-scrollable::-moz-scrollbar {
    display: none;
}

.preview-scrollable {
    height: 306px;
    cursor: move;
    touch-action: none;
    border-radius: 5px 5px 0 0;

    /* Disables scrolling */
    overflow: hidden;

    /* Removes IE scrollbars */
    -ms-overflow-style: none;
}

.side-box .preview-scrollable canvas.preview {
    border-radius: 0;
    position: relative;
    z-index: 2;
    cursor: move;
    width: auto;
    height: auto;
}
.preview-scrollable canvas.background {
    width: 100%;
    height: 100%;
    top: 0;
    position: absolute;
    z-index: 1;
}

.side-box.empty .preview-scrollable canvas.preview {
    cursor: pointer;
    position: absolute;
    width: 100%;
    height: 100%;
}
.preview + .data, .preview-scrollable + .data {
    visibility: hidden;
    width: auto;
    height: auto;
    position: absolute;
    left: 0;
    z-index: -1;
}
.data::selection, .feedback-box textarea::selection {
    color: #5581b5;
    background: rgba(255, 255, 255, 0.99);
}
.side.error .data::selection {
    color: rgba(85, 129, 181, 0.5);
    background: rgba(255, 255, 255, 0.99);
}
.data::-webkit-scrollbar-corner, .binary-textarea-content::-webkit-scrollbar-corner {
    background: transparent;
}
.data::-webkit-scrollbar-thumb, .binary-textarea-content::-webkit-scrollbar-thumb, .feedback-box textarea::-webkit-scrollbar-thumb, .combinator-list::-webkit-scrollbar-thumb, .text-sample span::-webkit-scrollbar-thumb {
    border-radius: 6px;
    background: white;
}
.data::-webkit-scrollbar, .binary-textarea-content::-webkit-scrollbar, .feedback-box textarea::-webkit-scrollbar, .combinator-list::-webkit-scrollbar, .text-sample span::-webkit-scrollbar {
    width: 6px;
    height: 6px;
}
.data::-webkit-scrollbar-track, .binary-textarea-content::-webkit-scrollbar-track, .feedback-box textarea::-webkit-scrollbar-track, .combinator-list::-webkit-scrollbar-track, .text-sample span::-webkit-scrollbar-track {
    background: rgba(0, 0, 0, 0.15);
    border-radius: 6px;
}
.side .badge {
    transition: opacity 0.2s ease, top 0.2s ease;
    visibility: hidden;
    width: 100%;
    font-size: 16px;
    min-height: 60px;
    border-radius: 4px;
    padding: 6px;
    font-family: "Roboto";
    top: -10px;
    user-select: none;
    left: 0;
    opacity: 0.25;
    padding-left: 55px;
    position: absolute;
    z-index: 999;
}
.badge-body {
    width: 100%;
    height: 100%;
}
.badge:before {
    content: '';
    position: absolute;
    width: 0;
    height: 0;
    top: -16px;
    border-top: 8px transparent solid;
    border-left: 8px transparent solid;
    border-right: 8px transparent solid;
    border-bottom: 8px transparent solid;
    left: 24px;
    transform: translateX(-10px);
}
.badge .badge-body .badge-title {
    font-weight: bold;
    text-shadow: 0 1px 0 black;
}
.badge-negative .badge {
    background: linear-gradient(to right, #b10000 0%, red);
    box-shadow: 0 3px 0 0 maroon;
    visibility: visible;
    top: 0;
    opacity: 1;
}
.badge-negative .badge:before {
    border-bottom: 8px #b10000 solid;
}
.badge-positive .badge {
    background: linear-gradient(to right, #10c104 0%, #14f105);
    box-shadow: 0 3px 0 0 green;
    visibility: visible;
    top: 0;
    opacity: 1;
}
.badge-positive .badge:before {
    border-bottom: 8px #10c104 solid;
}
.badge-positive .badge-icon:after {
    content: "";
    position: absolute;
    left: 21px;
    top: 14px;
    transform: rotate(45deg);
    width: 8px;
    border-bottom: 6px white solid;
    height: 20px;
    border-right: 6px white solid;
}
.badge-negative .badge-icon:after {
    content: "";
    position: absolute;
    left: 25px;
    top: 16px;
    transform: rotate(45deg);
    height: 28px;
    border-right: 6px white solid;
}
.badge-negative .badge-icon:before {
    content: "";
    position: absolute;
    left: 25px;
    top: 16px;
    transform: rotate(-45deg);
    height: 28px;
    border-right: 6px white solid;
}
.badge-warning .badge {
    background: linear-gradient(to right, #c7ac00 0%, #ebdf00);
    box-shadow: 0 3px 0 0 #9c9217;
    visibility: visible;
    top: 0;
    opacity: 1;
}
.badge-warning .badge:before {
    border-bottom: 8px #c7ac00 solid;
}
.badge-warning .badge-icon:after {
    content: "";
    position: absolute;
    left: 25px;
    top: 41px;
    height: 5px;
    border-right: 6px white solid;
}
.badge-warning .badge-icon:before {
    content: "";
    position: absolute;
    left: 25px;
    top: 16px;
    height: 21px;
    border-right: 6px white solid;
}
.badge-negative .badge ~ .side-wrapper .data, .badge-positive .badge ~ .side-wrapper .data , .badge-warning .badge ~ .side-wrapper .data {
    padding-top: 65px;
}
/* ----- Converter styling end ----- */





/* ----- Converter options styling ----- */
.option-group select {
    background: rgba(0, 0, 0, 0.15);
    color: white;
    border: 0;
    width: auto;
    max-width: 100%;
    position: relative;
    top: -3px;
    font-size: 15px;
    border-radius: 3px;
    box-shadow: inset 0 0 3px 0 rgba(0, 0, 0, 0.75), 0 0 0 1px rgba(255, 255, 255, 0.15);
    height: 24px;
    display: block;
    outline: none;
    font-family: "Roboto";
}
.select-wrapper {
    position: absolute;
    right: 0px;
    left: 30px;
    width: auto;
}
.select-wrapper ~ span.option-details {
    margin-top: 26px;
}
.option-group label {
    display: block;
}
[type="radio"],
[type="checkbox"] {
    position: absolute;
    left: -9999px;
}
.example-required-options-text {
    padding-bottom: 2px;
}
.option-row.option-resetter .icon,
.option-row.option-resetter .svg-icon {
    position: absolute;
    top: -1px;
    left: 2px;
    width: 20px;
    height: 20px;
    fill: white;
    opacity: 0.75;
}
[type="radio"] + label,
[type="checkbox"] + label, .option-row.option-resetter label {
    position: relative;
    padding-bottom: 6px;
    line-height: 16px;
    padding-left: 30px;
    cursor: pointer;
}
[type="radio"] + label:before,
[type="checkbox"] + label:before {
    content: '';
    position: absolute;
    left: 2px;
    top: 8px;
    transform: translateY(-50%);
    width: 0px;
    height: 0px;
    border: 0px solid rgba(255, 255, 255, 0.75);
    background-color: transparent;
}
[type="radio"] + label:hover:before, [type="checkbox"] + label:hover:before {
    border: 2px solid white;
}
[type="radio"]:checked + label:hover:after {
    background-color: white;
}
[type="checkbox"]:checked + label:hover:after {
    border-bottom: 3px solid white;
    border-right: 3px solid white;
}
[type="radio"]:checked + label:before,
[type="radio"]:not(:checked) + label:before {
    border-radius: 50%;
}
[type="radio"]:checked + label:after {
    position: absolute;
    content: '';
    top: 8px;
    transform: translateY(-50%);
    left: 6px;
    width: 0px;
    height: 0px;
    border-radius: 50%;
    background-color: rgba(255, 255, 255, 0.75);
}
[type="checkbox"]:checked + label:after {
    position: absolute;
    content: "";
    left: 8px;
    top: 2px;
    transform: rotate(45deg);
    width: 3px;
    border-bottom: 3px solid rgba(255, 255, 255, .75);
    height: 7px;
    border-right: 3px solid rgba(255, 255, 255, .75);
}
.option-group {
    display: inline-block;
    margin-right: 15px;
    vertical-align: top;
    min-width: 200px;
}
.option-row {
    display: block;
    position: relative;
    margin: 0 0 10px 0;
}

.option-group input[type="text"]:valid:focus + label, .option-group textarea:valid:focus + label {
    font-size: 10px;
}
.option-group input[type="text"] + label, .option-group textarea + label, .option-group .select-wrapper + label {
    display: block;
    position: absolute;
    top: -17px;
    left: 30px;
    font-size: 0;
}
.option-group input[type="text"]:valid, .option-group textarea:valid {
    color: white;
}

.option-group input[type="text"]::placeholder, .option-group textarea::placeholder {
    color: rgba(255, 255, 255, 0.5);
}
.option-group input[type="text"], .option-group textarea {
    background: rgba(0, 0, 0, 0.15);
    color: white;
    border: 0;
    margin: 10px 0px 0px 0px;
    position: relative;
    top: 7px;
    font-size: 22px;
    border-radius: 3px;
    box-shadow: inset 0 0 3px 0 rgba(0, 0, 0, 0.75), 0 0 0 1px rgba(255, 255, 255, 0.15);
    padding: 4px;
    height: 60px;
    width: 330px;
    display: block;
    outline: none;
    font-family: "arial";
}
.option-group textarea {
    resize: vertical;
    height: auto;
    min-height: 0px;
}
.option-group optgroup {
    background: #3c5c81;
    color: white;
    outline: none;
}
.option-group input[type="text"]:valid + label:before, .option-group textarea:valid + label:before, .option-group .select-wrapper + label:before {
    opacity: 1;
}
.option-group input[type="text"].color {
    width: 150px;
}
.option-group .icon_colorpicker {
    fill: white;
    position: absolute;
    left: 185px;
    height: 22px;
    width: 22px;
    cursor: pointer;
    top: -2px;
}
.option-group input[type="text"] + label:before, .option-group textarea + label:before, .option-group .select-wrapper + label:before {
    content: "";
    top: 13px;
    left: -26px;
    position: absolute;
    display: block;
    width: 18px;
    height: 22px;
    background-repeat: no-repeat;
    background-image: url(../images/icon-quote.png);
    opacity: 0.75;
}
span.option-details {
    margin-left: 30px;
    opacity: 0.6;
    padding-top: 3px;
    display: inline-block;
    vertical-align: top;
    white-space: pre-line;
    font-size: 13px;
    position: relative;
    top: -5px;
}


.examples .option-group b {
    text-shadow: 0px 1px 0px black;
    display: inline-block;
    padding-top: 5px;
}
.examples .option-group {
    display: block;
    margin: 10px 0 0 0;
    border-top: 1px rgba(255, 255, 255, 0.2) dotted;
}
.examples .option-row {
    margin: 5px 0 0 0;
}

.option-row.compact-2 input[type="text"],
.option-row.compact-2 .option-details {
    width: 85px;
}

.option-row.compact-3 input[type="text"],
.option-row.compact-3 .option-details {
    width: 55px;
}

.option-row.is-compact .option-details {
    //white-space: nowrap;
    text-overflow: ellipsis;
    overflow: hidden;
}

.option-row.is-compact input[type="text"]:focus + label {
    //font-size: 0;
}

.option-row.is-compact {
    display: inline-block;
}

.option-row.is-compact + .option-row.is-compact input,
.option-row.is-compact + .option-row.is-compact .option-details,
.option-row.is-compact + .option-row.is-compact label {
    margin-left: 0;
    left: 0;
}

.option-row.is-compact + .option-row.is-compact label::before {
    display: none;
}

.option-row.is-comment label:before {
    content: "";
    top: -5px;
    left: 3px;
    position: absolute;
    display: block;
    width: 18px;
    height: 22px;
    background-repeat: no-repeat;
    opacity: 0.75;
    background-image: url(../images/icon-question.png);
}
/* ----- Converter options styling end ----- */





/* ----- About this tool styling, all tools... ----- */
@keyframes cursor-blink {
    0% {
        opacity: 0.5;
    }
    50% {
        opacity: 0.5;
    }
    51% {
        opacity: 0;
    }
    100% {
        opacity: 0;
    }
}

.pro-tip .url {
    background: white;
    text-overflow: ellipsis;
    overflow: hidden;
    max-height: 95px;
    word-break: break-all;
    border: 1px #a9a9a9 solid;
    border-radius: 3px;
    line-height: 22px;
    font-size: 14.5px;
    padding: 4px;
}
.pro-tip .omnibox {
    background: #f2f2f2;
    margin: 8px 0 14px 0;
    padding: 5px;
    cursor: pointer;
    user-select: none;
    box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
    border-radius: 3px;
    position: relative;
}
.pro-tip .url .muted {
    opacity: 0.7;
}
.pro-tip .green {
    color: forestgreen;
}

/* .pro-tip .navigation {
    position: absolute;
    left: 0;
    height: 42px;
    font-size: 0;
    padding-left: 5px;
    top: 50%;
    transform: translateY(-50%);
}
.pro-tip .navigation i {
    padding-top: 9px;
    opacity: 0.75;
    padding-right: 6px;
} */


body .section.all-tools .secondary {
    opacity: 1;
    position: relative;
}
.all-tools .secondary .search:focus + .cursor,  .all-tools .secondary .search:valid + .cursor{
    display: none;
}
.all-tools .secondary .search {
    opacity: 0.5;
    border: 0;
    width: 100%;
    outline: 0;
    font-family: "Roboto";
    font-size: 27px;
    font-weight: bold;
    color: black;
}
.all-tools .tool-matches-amount:empty {
    display: none;
}
.all-tools .tool-matches-amount {
    position: absolute;
    color: white;
    background: crimson;
    z-index: 99;
    display: inline-block;
    border-radius: 19px;
    left: -22px;
    line-height: 19px;
    padding: 0px 6px 0px 6px;
}
.all-tools .tool-none-matches {
    width: 100%;
    height: 100%;
    padding-left: 10px;
    padding-top: 10px;
    position: absolute;
    font-size: 16px;
    z-index: 99;
    opacity: 0;
    transition: all 0.2s ease;
    background: rgba(255, 255, 255, 0.75);
    visibility: hidden;
}
.tool-none-matches .request-tool, .section.tool-unlisted .unlisted-feedback {
    text-decoration: underline;
    cursor: pointer;
}
.tool-none-matches .message {
    display: inline-block;
    padding: 15px;
    color: white;
    background: #5581b5;
    box-shadow: 0px 3px 0 0 #2e4765;
    border-radius: 3px;
}
.tool-none-matches .message:before {
    top: -6px;
    left: 30px;
}
.tool-none-matches a {
    color: white;
}
.all-tools .tool-none-matches.active {
    visibility: visible;
    opacity: 1;
}
.all-tools .secondary .search:focus, .all-tools .secondary .search:valid{
    opacity: 0.75;
}
.all-tools .secondary .cursor {
    animation: cursor-blink 1.2s infinite linear;
    width: 1px;
    height: 33px;
    display: block;
    position: absolute;
    left: 4px;
    top: 3px;
    background: black;
}
.all-tools .secondary .search::placeholder {
    color: black;
}
/* ----- About this tool styling, all tools... end ----- */





/* ----- Cards styling ----- */
.cards {
    font-size: 0;
    margin-left: -10px;
    position: relative;
    padding-bottom: 3px;
    display: flex;
    flex-wrap: wrap;
}
.card .title a {
    text-decoration: none;
    color: white;
}
.cards .card {
    transition: opacity 0.25s ease;
    vertical-align: top;
    width: 33.333%;
    display: inline-block;
    padding: 10px 0px 0px 10px;
    font-size: 16px;
}

.cards .card .block {
    cursor: pointer;
    user-select: none;
    height: 100%;
    transition: box-shadow 0.2s ease;
    background: #5581b5;
    color: white;
    box-shadow: 0px 3px 0 0 #2e4765;
    border-radius: 3px;
    padding: 4px 8px;
}
.cards .card:not(.hidden) .block:hover {
    box-shadow: 0px 3px 0 0 #2e4765, 0 14px 28px rgba(0,0,0,0.25), 0 10px 10px rgba(0,0,0,0.22);
}
.cards .card .block .title {
    text-shadow: 0px 1px 0px black;
    padding-right: 25px;
    position: relative;
    font-weight: bold;
    padding-bottom: 2px;
    border-bottom: 1px rgba(255, 255, 255, 0.2) dotted;
}
.cards .card .block .arrow {
    position: absolute;
    top: 0px;
    right: 0px;
}
.cards .card .block .arrow svg {
    fill: white;
    width: 25px;
    height: 25px;
}
.coming-soon-list.cards .card .block {
    background: #9e9e9e;
    box-shadow: 0px 3px 0 0 #6f6f6f;
}
.coming-soon-list.cards .card .block:hover {
    box-shadow: 0px 3px 0 0 #6f6f6f, 0 14px 28px rgba(0,0,0,0.25), 0 10px 10px rgba(0,0,0,0.22);
}
.cards .card .block .body {
    padding-top: 2px;
}
.examples.cards .card .block .title .open-in-new {
    position: absolute;
    top: 2px;
    right: 0px;
}
.examples.cards .card .block .title .open-in-new svg {
    fill: white;
    width: 20px;
    height: 20px;
}
.examples .wrapper {
    text-align: center;
    margin: 5px;
}
.sample .input-sample, .sample .output-sample {
    display: inline-block;
    font-family: "SFMono-Regular", Consolas, "Liberation Mono", Menlo, Courier, monospace;
    position: relative;
    text-align: left;
    font-size: 14px;
    border-radius: 3px;
    padding: 3px;
    background: rgba(0, 0, 0, 0.25);
    box-shadow: inset 0 0 3px 0 rgba(0, 0, 0, 0.75), 0 0 0 1px rgba(255, 255, 255, 0.15);
}
.sample .text-sample span {
    white-space: pre-wrap;
    max-height: 295px;
    display: inline-block;
    vertical-align: top;
    overflow-x: hidden;
    overflow-y: auto;
    width: 100%;
    text-overflow: ellipsis;
}
.sample {
    display: inline-flex;
    position: relative;
    align-items: center;
}
.sample.big {
    margin-right: 15px;
    display: block;
}
.sample.big .input-sample, .sample.big .output-sample {
    display: block;
}
.sample .input-sample {
    margin-right: 23px;
}
.sample.big .input-sample {
    margin-bottom: 8px;
    margin-right: 0;
}

/* Hides the arrow and output if there's no output,
   Hides the input if there's no input,
   Hides itself if there's no input and output */
.sample.without-output .input-sample:after, .sample.without-output .output-sample, .sample.without-output.without-input, .sample.without-input .input-sample {
    display: none;
}
.sample .input-sample:after {
    content: "";
    position: absolute;
    right: -21px;
    bottom: 50%;
    transform: translateY(50%);
    background-image: url(../images/icon-arrows.png);
    width: 17px;
    height: 21px;
    background-position-x: -26px;
    background-repeat: no-repeat;
    background-size: cover;
}
.sample.big .input-sample:after {
    background-position-x: 0;
    transform: none;
    bottom: -17px;
    right: -23px;
    width: 25px;
    height: 25px;
}
.examples .sample .image-sample {
    padding: 0;
    white-space: normal;
}
.sample .image-sample img {
    max-width: 100%;
    max-height: 100%;
    display: block;
    border-radius: 3px;
    margin: 0 auto;
}
.file-sample .file-icon {
    width: 40px;
    height: 50px;
    margin-bottom: 5px;
    background: white;
    position: relative;
    border-radius: 2px;
    display: inline-block;
}

.sample .file-sample {
    padding: 0;
    border-radius: 0;
    box-shadow: none;
    background: transparent;
}

.file-sample .file-icon:after {
    content: "";
    position: absolute;
    top: 0;
    right: 0;
    border-width: 0 16px 16px 0;
    border-style: solid;
    border-color: transparent #5581b5 rgba(0, 0, 0, 0.2) transparent;
    border-radius: 0 0 0 3px;
    background: white;
    display: block;
    width: 0;
}

.file-sample .file-description {
    position: absolute;
    left: 55px;
    right: 0;
    display: inline-block;
}

.file-sample .file-header {
    position: relative;
}

.file-description .file-title, .file-description .file-subtitle {
    text-overflow: ellipsis;
    white-space: nowrap;
    overflow: hidden;
    font-family: "Roboto";
}

.file-description .file-title {
    font-weight: bold;
    text-shadow: 0 1px black;
    font-size: 18px;
}

.file-sample .file-content {
    font-family: monospace;
    position: relative;
    text-align: left;
    font-size: 14px;
    border-radius: 3px;
    padding: 3px;
    background: rgba(0, 0, 0, 0.25);
    box-shadow: inset 0 0 3px 0 rgba(0, 0, 0, 0.75), 0 0 0 1px rgba(255, 255, 255, 0.15);
}

.file-description .file-subtitle {
    font-size: 15px;
}
.cards .card.hidden {
    opacity: 0.4;
}
.card.favorite .block .title:before {
    content: "star";
    color: #f7d000;
    position: absolute;
    right: 27px;
    top: 1px;
    font-family: 'Material Icons';
    font-size: 20px;
    display: inline-block;
    line-height: 1;
    white-space: nowrap;
    -webkit-font-smoothing: antialiased;
    text-rendering: optimizeLegibility;
    -moz-osx-font-smoothing: grayscale;
    font-feature-settings: 'liga';
}
/* ----- Cards styling end ----- */





/* ----- Subscribe box styling ----- */
.fullwidth-wrapper.show-notification.shadow-lock {
    box-shadow: 0 0 0 999em rgba(0, 0, 0, 0.5), 0 0 5px 0 rgba(0, 0, 0, 0.5);
    z-index: 999;
}
.fullwidth-wrapper {
    transition: box-shadow 0.2s ease;
    background: #e05745;
    padding-top: 10px;
    padding-bottom: 20px;
    position: relative;
}
.fullwidth-wrapper .notification, .fullwidth-wrapper.show-notification .subscription {
    display: none;
}
.fullwidth-wrapper.show-notification .notification {
    display: block;
}
.subscribe.notification .onlinetools-subscribe-box button {
    display: inline-block;
    position: relative;
    width: 50%;
    padding: 14px;
    border-radius: 0;
    box-shadow: inset 0px 6px 6px -6px rgba(0, 0, 0, 0.5);
}

.subscribe.notification .onlinetools-subscribe-box input {
    border-radius: 4px 4px 0 0;
}
.content .section.subscribe .icon {
    color: white;
}
.subscribe .onlinetools-subscribe-box {
    margin-top: 9px;
    width: 48%;
    background: transparent;
    border-radius: 4px;
    position: relative;
    display: block;
    font-size: 0;
    box-shadow: 0px 4px 0px 0px #863025;
}
.onlinetools-subscribe-box .onlinetools-subscribe-form, .feedback-box .feedback-form, .onlinetools-subscribe-box.complete .subscribe-success, .feedback-box.complete .feedback-success, .feedback-box.error .feedback-error {
    display: block;
}
.onlinetools-subscribe-box .subscribe-success, .onlinetools-subscribe-box.complete .onlinetools-subscribe-form, .feedback-box .feedback-success, .feedback-box .feedback-error, .feedback-box.complete .feedback-form, .feedback-box.error .feedback-form {
    display: none;
}
.subscribe .body .onlinetools-subscribe-box:before {
    border-bottom: 8px white solid;
}
.subscribe .body .onlinetools-subscribe-box.complete:before {
    border-bottom: 8px rgba(0, 0, 0, 0.25) solid;
}
.subscribe .body .primary {
    color: white;
}
.subscribe .onlinetools-subscribe-box button {
    position: absolute;
    top: 0;
    right: 0;
    font-family: "Roboto";
    outline: none;
    font-size: 16px;
    color: white;
    border: none;
    background: #b74839;
    padding: 17px 14px 16px 15px;
    border-radius: 0 3px 3px 0;
    font-weight: bold;
    text-shadow: 0px 1px 0px black;
    cursor: pointer;
    box-shadow: inset 6px 0px 6px -6px rgba(0, 0, 0, 0.5);
}
.subscribe .onlinetools-subscribe-box input {
    font-family: "Roboto";
    outline: none;
    border: none;
    font-size: 18px;
    padding: 15px 10px 15px 10px;
    border-radius: 4px;
    background: white;
    width: 100%;
    color: black;
}
.subscribe .subscribe-success {
    width: 100%;
    padding: 13px 10px 12px 10px;
    color: white;
    background: rgba(0, 0, 0, 0.25);
    font-size: 18px;
    border-radius: 4px;
}
.feedback .feedback-success {
    padding: 13px 10px 12px 10px;
    color: white;
    background: rgba(0, 0, 0, 0);
    font-size: 18px;
    border-radius: 5px;
    box-shadow: 0px 4px 0 0 rgb(46, 71, 101);
}

#feedback-error-message {
    white-space: pre;
    padding: 13px 10px 12px 10px;
    color: white;
}
/* ----- Subscribe box styling end ----- */





/* ----- Footer styling ----- */
.feedback .feedback-box input::placeholder, .feedback .feedback-box textarea::placeholder {
    color: rgba(255, 255, 255, 0.5);
}
.feedback .feedback-box input[type="text"] {
    border-bottom: 1px rgba(255, 255, 255, 0.2) dotted;
}

.feedback .feedback-button {
    border: 0;
    font-family: "Roboto";
    outline: none;
    cursor: pointer;
    display: block;
    width: 100%;
    padding: 16px;
    font-size: 16px;
    background: #476c98;
    border-radius: 0px 0px 4px 4px;
    box-shadow: inset 0px 6px 6px -6px rgba(0, 0, 0, 0.5), 0px 4px 0 0 rgb(46, 71, 101);
    color: white;
    font-weight: bold;
    text-shadow: 0px 1px 0px black;
}
.feedback .feedback-box input, .feedback .feedback-box textarea {
    border: 0;
    color: white;
    resize: none;
    display: block;
    font-size: 18px;
    padding: 15px 10px 15px 10px;
    width: 100%;
    background: transparent;
    font-family: "Roboto";
    outline: none;
}
.feedback .feedback-box textarea {
    margin-top: 10px;
    margin-bottom: 5px;
    margin-right: 5px;
    width: 99%;
    padding-top: 0;
    height: 150px;
}
.feedback .feedback-box {
    position: relative;
    width: 48%;
    background: #5581b5;
    border-radius: 5px;
    margin-top: 10px;
}
.created-by .primary {
    vertical-align: middle;
}

.created-by .fffff-and-ttttt {
    display: inline-block;
}

.section.created-by i.icon {
    color: rgba(237, 20, 20, 0.35);
}

/* For footer padding only */
.footer {
    font-family: "Roboto";
}
.footer.container .content {
    margin-top: 40px;
    margin-bottom: 40px;
}

.browserling-logo {
    margin-left: 5px;
    margin-right: 10px;
}
.browserling-logo img {
    vertical-align: middle;
}

/* ----- Footer styling end ----- */





/* ----- Secret section styling ----- */
.secret {
    opacity: 0.30;
}
.secret.section .icon {
    opacity: 1;
}
.secret.section .primary {
    color: black;
}
.secret .coupon-code {
    color: #e05745;
}
/* ----- Secret section styling end ----- */




/* ----- Privacy policy section and ToS styling ----- */
.privacy-policy, .tos {
    opacity: 0.8;
}
.privacy-policy.section .body-content,
.tos.section .body-content {
    font-size: 14px;
}
/* ----- Privacy policy section and ToS styling end ----- */




/* ----- Responsive override ----- */

/* When on small screens (tablets) */
@media(max-width: 992px) {
    .container {
        width: 85%;
    }
    .logo {
        margin: 0 auto;
        display: block;
    }
    .sides .side.input, .sides .side.input + .side.output {
        clear: both;
        width: 100%;
    }
    .side.output {
        margin-top: 20px;
    }
    .sides .tool-inline .tool-toggle-layout {
        display: none;
    }
    .sides .side label .side-layout {
        display: none;
    }
    .section .onlinetools-subscribe-box, .section .feedback-box {
        width: 100%;
    }
    
    .section .onlinetools-subscribe-box input {
        width: 100%;
        padding-right: 100px;
        border-radius: 4px;
    }
    
    .section .onlinetools-subscribe-box button {
        position: absolute;
        right: 0;
    }
    .cards .card {
        width: 50%;
    }
    .tool:nth-child(odd) .chain-link {
        right: -45px;
    }
    .tool:nth-child(even) .chain-link {
        left: -45px;
    }
    .tool:last-child .chain-link {
        display: none;
    }
}

/* When on really small screens */
@media(max-width: 767px) {
    /*.side-widgets .side-widgets-wrapper:after, .side-widgets .side-widgets-toggle:after {
        display: none;
    }
    .side-widgets.toggled .side-widgets-toggle, .side-widgets .side-widgets-wrapper {
        visibility: visible;
    }
    .side-widgets.toggled .side-widgets-wrapper, .side-widgets .side-widgets-toggle {
        visibility: hidden;
    }
    .side-widgets .side-widgets-wrapper, .side-widgets .side-widgets-toggle {
        transform: none!important;
    }*/
    .side.output {
        margin-top: 20px;
    }
    .tool:nth-child(even) .chain-link, .tool:nth-child(odd) .chain-link {
        position: absolute;
        display: block;
        left: -40px;
        top: 235px;
        border: 5px #d1d1d1 dashed;
        border-right: none;
        width: 20px;
        border-radius: 5px 0 0 5px;
        height: auto;
        bottom: -225px;
    }
    .tool:nth-child(odd) .chain-link:after, .tool:nth-child(even) .chain-link:after {
        content: "";
        bottom: -8px;
        display: block;
        position: absolute;
        right: -10px;
        left: auto;
        width: 0;
        height: 0;
        border-bottom: 6px solid transparent;
        border-top: 6px solid transparent;
        border-left: 10px solid #d1d1d1;
        border-right: none;
        font-size: 0;
        line-height: 0;
    }
    .tool:last-child .chain-link {
        display: none;
    }
    .cards .card {
        width: 100%;
    }
    .container {
        width: auto;
        margin-left: 10px;
        margin-right: 10px;
    }

    .header img {
        height: auto;
        max-width: 100%;
    }
    .container .content {
        margin-left: 49px;
    }
    .section > .icon {
        left: -49px;
    }
    .section .body .secondary {
        padding-left: 0;
    }

    .section .onlinetools-subscribe-box button {
        box-shadow: inset 0px 6px 6px -6px rgba(0, 0, 0, 0.5);
        width: 100%;
        border-radius: 0;
        padding: 10px 0 10px 0;
        position: relative;
    }

    .section .onlinetools-subscribe-box input {
        border-radius: 4px 4px 0 0;
        padding-right: 10px;
    }
}

/* At this width, no longer float the menu right */
@media(max-width: 715px) {
    .header .left-side {
        float: none;
    }
    .header .right-side {
        float: none;
        margin-top: 6px;
    }
}

/* At this width, split the logo and the fb like button apart */
@media(max-width: 450px) {
    .header .left-side .logo {
        display: block;
    }
    .header .left-side .fffff {
        left: 0px;
        margin-top: 6px;
    }
}
/* ----- Responsive override end ----- */

.fffff {
    color: white;
    font-family: Helvetica, Arial, sans-serif;
    background: #1877f2;
    font-size: 11px;
    height: 20px;
    padding: 2px 10px 0px 6px;
    border-radius: 3px;
    display: inline-block;
    vertical-align: middle;
    cursor: pointer;
}

.fffff:before {
    content: "Like";
    font-weight: bold;
    height: 16px;
    display: inline-block;
    padding: 0px 4px 0 20px;
    background-repeat: no-repeat;
    background-size: 16px 16px;
    background-image: url("data:image/svg+xml,%3Csvg fill='white' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3E%3Cpath fill-rule='evenodd' d='M4.5 7c.3 0 .5.2.5.5v6c0 .3-.2.5-.5.5h-2c-.3 0-.5-.2-.5-.5v-6c0-.3.2-.5.5-.5h2zm2 6.2c-.3 0-.5-.3-.5-.6V8c0-.5.1-1.4.4-1.8l1.5-2c.3-.5.6-.8.6-1.1v-.8c0-.5.2-.9.8-.9.2 0 .4 0 .6.3.3.4.5 1 .5 1.8 0 .9-.9 2.6-.9 2.6h4c.7 0 1 .5 1 1.1 0 .5-.4 1-.8 1 .2.2.5.5.5 1 0 .4-.4.8-.8.8l.4.7c0 .4-.3.8-.6.9.2.1.3.4.3.6 0 .5-.3.9-.8.9H6.5z'/%3E%3C/svg%3E");
}

.ttttt {
    color: white;
    font-family: "Helvetica Neue", Arial, sans-serif;
    background: #1b95e0;
    font-size: 11px;
    height: 20px;
    padding: 2px 8px 1px 6px;
    border-radius: 3px;
    display: inline-block;
    vertical-align: middle;
    cursor: pointer;
}

.ttttt:before {
    content: "Follow";
    display: inline-block;
    padding: 0px 3px 0 18px;
    background-repeat: no-repeat;
    background-position-y: 1px;
    background-size: 14px 14px;
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 72 72'%3E%3Cpath fill='%23fff' d='M68.8 15.1c-2.3 1-4.9 1.8-7.5 2.1C64 15.6 66 13 67 10a26.1 26.1 0 01-8.3 3.1 13 13 0 00-22.3 12 37.2 37.2 0 01-27-13.7 13 13 0 004 17.5 13 13 0 01-5.8-1.7v.2C7.6 33.7 12 39 18 40.2a13.2 13.2 0 01-6 .3c1.7 5.2 6.6 9 12.3 9A26.3 26.3 0 015 55a37 37 0 0057.3-33c2.5-2 4.8-4.2 6.5-6.9z'/%3E%3C/svg%3E");
}
