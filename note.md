---
title: Dark Theme
description: A dark theme for HackMD
tags: Theme
---

<!--
  A dark theme for HackMD.

  To use, append `{%hackmd @Luminous-Coder/dark-theme %}` at the end of the note.
  If you don't like the style of the license, it is `#lmn-dark-theme-license`, so you can change the style.

  Icons:
    Use the class `lmn-icon` to display FontAwesome icons. You can find the list here: https://fontawesome.com/search.
    Example: <span class="lmn-icon">&#xF05A;</span>

  Version Annotations:
    Use the classes `lmn-vs` for version specific contents and `lmn-va` for version annotations.
    Inspired by cppreference.
-->

<style>
    /* Background */
    body {
        background-color: #1E1E1E !important;
        text-shadow: none;
    }
    
    .ui-view-area, .ui-content, .markdown-body {
        background-color: #1E1E1E;
        color: #FFFFFF;
    }
    
    /* Buttons */
    .btn-default {
        background-color: transparent;
        color: #D0D0D0;
        border: 1px solid #696969;
    }
    
    .btn-default:hover {
        background-color: transparent;
        color: #FFFFFF;
        border: 1px solid #696969;
    }
    
    .btn-primary.btn-outline {
        color: #10A0FF;
        border-color: #10A0FF;
    }
    
    .btn-primary.btn-outline:hover {
        background-color: transparent;
        color: #00A6FF;
        text-shadow: 0 0 0.1em #00A6FF;
        border-color: #00A6FF;
        box-shadow: 0 0 0.3em #00A6FF;
    }
    
    .btn-danger {
        background-color: transparent;
        color: #D9534F;
        border-color: #D95345;
    }
    
    .btn-danger:hover {
        background-color: transparent;
        color: #D9534F !important;
        text-shadow: 0 0 0.1em #D9534F;
        border-color: #D9534F;
        box-shadow: 0 0 0.3em #D9534F;
    }
    
    /* Dropdown Menus */
    .dropdown-menu {
        background-color: #000000;
        border: 1px solid #696969;
    }
    
    .dropdown-menu .dropdown-header {
        color: #C5C5C5;
    }
    
    .dropdown-menu .divider {
        border-bottom-color: #555555 !important;
    }
    
    .dropdown-menu > li {
        color: #D0D0D0;
    }
    
    .dropdown-menu > li > a,
    .dropdown-menu > li > a:focus {
        background-color: transparent;
        color: #D0D0D0;
    }
    
    .dropdown-menu > li > a:hover {
        background-color: transparent;
        color: #FFFFFF;
        text-shadow: 0 0 0.1em #FFFFFF;
    }
    
    .menuitem-dropdown .menuitem-dropdown-trigger {
        background-color: transparent;
        color: #D0D0D0;
        border-color: #696969;
    }
    
    .menuitem-dropdown .menuitem-dropdown-trigger:hover,
    .menuitem-dropdown .menuitem-dropdown-trigger:focus {
        background-color: transparent;
        color: #FFFFFF;
        text-shadow: 0 0 0.1em #FFFFFF;
    }
    
    .menuitem-dropdown .menuitem-dropdown-trigger.disabled {
        color: #696969;
        opacity: 1;
    }
    
    /* Form Controls */
    .form-control {
        background-color: transparent;
        color: #D0D0D0;
        border-color: #696969;
    }
    
    .form-control::placeholder {
        color: #D0D0D0;
    }
    
    .form-control:hover, .form-control:focus {
        background-color: transparent;
        color: #FFFFFF;
        border-color: #FFFFFF;
    }
    
    .form-control:hover::placeholder, .form-control:focus::placeholder {
        color: #FFFFFF;
    }
    
    /* Tooltips */
    .ui-first-menu-tooltip, .ui-second-menu-tooltip {
        color: #696969 !important;
    }
    
    .ui-first-menu-tooltip:hover, .ui-second-menu-tooltip:hover {
        color: #FFFFFF !important;
        text-shadow: 0 0 0.2em #FFFFFF;
    }
    
    /* Navigate Bar */
    .navbar {
        background-color: #000000;
        border: none;
    }
    
    .navbar-default .navbar-brand {
        color: #C5C5C5;
    }
    
    .navbar-default .navbar-brand:hover {
        color: #FFFFFF;
    }
    
    .ui-edit:hover, .ui-both:hover, .ui-view:hover,
    .ui-edit:active, .ui-both:active, .ui-view:active,
    .ui-edit:hover:active, .ui-both:hover:active, .ui-view:hover:active,
    .ui-edit.active, .ui-both.active, .ui-view.active,
    .ui-edit.active:hover, .ui-both.active:hover, .ui-view.active:hover,
    .ui-edit.active.focus, .ui-both.active.focus, .ui-view.active.focus {
        background-color: #303030;
        color: #FFFFFF;
        text-shadow: 0 0 0.5em #FFFFFF;
        border-color: #696969;
    }
    
    .ui-infobar .btn.ui-edit {
        background-color: #000000;
        color: #D0D0D0;
        border-color: #696969;
    }
    
    .ui-infobar .btn.ui-edit:hover {
        background-color: #303030;
        color: #FFFFFF;
    }
    
    .navbar-default .navbar-nav > li > a,
    .navbar-default .navbar-nav > li > a:focus {
        background-color: transparent;
        color: #C5C5C5;
    }
    
    .navbar-default .navbar-nav > li > a:hover {
        background-color: transparent !important;
        color: #FFFFFF;
    }
    
    .navbar-default .navbar-nav > li.open > a,
    .navbar-default .navbar-nav > li.open > a:focus,
    .navbar-default .navbar-nav > li.open > a:hover {
        background-color: transparent;
        color: #FFFFFF;
    }
    
    .navbar-default .announcement-area .caption.inverse {
        color: #C5C5C5;
    }
    
    .navbar-default .announcement-area .caption.inverse:hover {
        color: #FFFFFF;
    }
    
    .navbar-right .btn.ui-status.online {
        color: #C5C5C5;
    }
    
    .navbar-right .btn.ui-status.online:hover,
    .navbar-right .ui-host-list.open .btn.ui-status.online {
        background-color: transparent;
        color: #FFFFFF;
    }
    
    .navbar-right .btn.ui-sharing.signin {
        background-color: transparent;
        color: #5CB85C;
    }
    
    .navbar-right .ui-profile-label:hover .ui-avatar {
        box-shadow: 0 0 5px #FFFFFF;
    }
    
    .navbar-right .btn.ui-sharing.signin:hover,
    .navbar-right .ui-share-button.open .btn.ui-sharing.signin {
        background-color: transparent;
        box-shadow: 0 0 5px #5CB85C;
    }
    
    .input-group .input-group-btn .ui-share-copy {
        background-color: transparent;
        color: #D0D0D0;
        border-color: #696969;
    }
    
    .input-group .input-group-btn .ui-share-copy:hover {
        background-color: transparent;
        color: #FFFFFF;
        text-shadow: 0 0 0.1em #FFFFFF;
    }
    
    .permission-dropdown .ui-share-preview {
        background-color: transparent;
        color: #D0D0D0;
        border-color: #696969;
    }
    
    .permission-dropdown .ui-share-preview:hover {
        background-color: transparent;
        color: #FFFFFF;
        text-shadow: 0 0 0.1em #FFFFFF;
    }
    
    .permission-dropdown .ui-more-settings {
        color: #10A0FF !important;
    }
    
    .permission-dropdown .ui-more-settings:hover {
        color: #10A0FF !important;
        text-shadow: 0 0 0.1em #10A0FF !important;
        text-decoration: none !important;
    }
    
    .ui-more-settings-menu-back {
        background-color: #000000 !important;
        color: #D0D0D0;
        border-bottom-color: #696969 !important;
    }
    
    .ui-more-settings-menu-back:hover {
        color: #FFFFFF;
        text-shadow: 0 0 0.2em #FFFFFF;
    }
    
    .ui-invitee-input {
        border-color: #696969;
    }
    
    .ui-invitee-input > .select2-choices {
        background-color: #000000;
        color: #D0D0D0;
    }
    
    .ui-invitee-input > .select2-choices:focus {
        color: #FFFFFF;
    }
    
    .ui-invitee-invite {
        background-color: transparent;
        color: #D0D0D0;
        border-color: #696969 !important;
    }
    
    .ui-invitee-invite:hover {
        color: #FFFFFF;
    }
    
    .public-published-toggle .publish,
    .public-published-toggle .unpublish-action,
    .public-published-toggle .unpublish {
        background-color: transparent;
        color: #D0D0D0;
        border: 1px solid #696969;
    }
    
    .public-published-toggle .publish:hover,
    .public-published-toggle .unpublish-action:hover,
    .public-published-toggle .unpublish:hover {
        color: #FFFFFF;
        text-shadow: 0 0 0.1em #FFFFFF;
    }
    
    /* Modal-Contents */
    .modal-content {
        background-color: #000000;
        border: 1px solid #696969;
    }
    
    .modal-content .modal-header {
        background-color: transparent;
        color: #D0D0D0;
        border-color: #696969;
    }
    
    .modal-content .modal-header .close {
        color: #D0D0D0;
        opacity: 1;
        text-shadow: none;
    }
    
    .modal-content .modal-header .close:hover {
        color: #FFFFFF;
    }
    
    .modal-content .modal-body {
        color: #FFFFFF !important;
    }
    
    /* Versions and GitHub Sync */    
    #namedRevisionModal .modal-title {
        color: #C5C5C5;
    }
    
    #namedRevisionModal .ui-github-sync {
        border-color: #696969 !important;
    }
    
    #namedRevisionModal .signin-to-connect,
    #namedRevisionModal .no-connect-github {
        color: #D0D0D0;
    }
    
    #namedRevisionModal .no-connect-github > a {
        color: #10A0FF;
    }
    
    #namedRevisionModal .no-connect-github > a:hover {
        color: #10A0FF;
        text-decoration: none;
        text-shadow: 0 0 0.1em #10A0FF;
    }
    
    #namedRevisionModal .github-status,
    #namedRevisionModal .github-status a {
        color: #D0D0D0;
    }
    
    #namedRevisionModal .github-status a:hover {
        color: #FFFFFF;
        text-decoration: none;
        text-shadow: 0 0 0.1em #FFFFFF;
    }
    
    #namedRevisionModal .sidebar.revision-list-container {
        border-color: #696969;
    }
    
    #namedRevisionModal .revision-card .revision-card-heading,
    #namedRevisionModal .revision-item {
        color: #D0D0D0;
    }
    
    #namedRevisionModal .revision-card .revision-card-heading:hover,
    #namedRevisionModal .revision-item:hover,
    #namedRevisionModal .revision-card.active .revision-card-heading,
    #namedRevisionModal .revision-item.active {
        background-color: transparent;
        color: #FFFFFF;
        text-shadow: 0 0 0.1em #FFFFFF;
    }
    
    #namedRevisionModal .ui-upgrade-tips {
        color: #C5C5C5;
        border-color: #696969;
    }
    
    #namedRevisionModal .ui-upgrade-tips .ui-upgrade-button {
        color: #10A0FF;
    }
    
    #namedRevisionModal .ui-upgrade-tips .ui-upgrade-button:hover {
        color: #10A0FF;
        text-decoration: none;
        text-shadow: 0 0 0.1em #10A0FF;
    }
    
    #namedRevisionModal .revision-item.preview {
        opacity: 1;
    }
    
    #namedRevisionModal #revisionSummary,
    #namedRevisionModal #revisionSummary h4,
    #namedRevisionModal #revisionSummary .summary-author-info,
    #namedRevisionModal #revisionSummary .summary-description,
    #namedRevisionModal #revisionSummary .tooltip-align-left {
        background-color: transparent;
        color: #C5C5C5 !important;
    }
    
    #namedRevisionModal #revisionSummary .tooltip-align-left:hover {
        color: #FFFFFF !important;
        text-shadow: 0 0 0.1em #FFFFFF;
    }
    
    #namedRevisionModal #revision-operation-panel {
        background-color: transparent;
    }
    
    #namedRevisionModal #diff-revision-dropdown-menu .btn:active,
    #namedRevisionModal #diff-revision-dropdown-menu .btn:focus {
        background-color: transparent;
        color: #FFFFFF;
        border-color: #696969;
    }
    
    #namedRevisionModal #diff-revision-dropdown-menu .section-header {
        background-color: transparent;
        color: #C5C5C5;
    }
    
    #namedRevisionModal .revision-card[disabled] .revision-card-heading:hover {
        background-color: transparent;
    }
    
    /* Tool Bar */
    .tool-bar {
        background-color: #101010;
    }
    
    .tool-bar > a {
        color: #868686 !important;
    }
    
    .tool-bar > a:hover {
        background-color: transparent;
        color: #FFFFFF !important;
        text-shadow: 0 0 0.1em #FFFFFF;
        border-color: transparent;
    }
    
    .tool-bar > a.active, .tool-bar > a.active:hover {
        background-color: transparent;
        color: #FFFFFF !important;
        text-shadow: 0 0 0.1em #FFFFFF;
        border-color: transparent;
    }
    
    /* Split Line in Both View */
    .ui-edit-area .ui-resizable-handle.ui-resizable-e {
        width: 6px;
        background-color: #696969;
        box-shadow: 0 0 6px #696969;
    }
    
    .ui-edit-area .ui-sync-toggle {
        box-shadow: 0 0 6px #D0D0D0;
    }
    
    .ui-edit-area .ui-sync-toggle:hover,
    .ui-edit-area .ui-sync-toggle:focus {
        background-color: transparent;
        color: #FFFFFF;
        box-shadow: 0 0 6px #D0D0D0;
    }
    
    /* Popover */
    .ui-user-icon.small:hover {
        box-shadow: 0 0 3px #FFFFFF;
    }
    
    .popover {
        background-color: #000000;
        border: 1px solid #696969;
    }
    
    .popover.bottom > .arrow {
        border-bottom-color: #696969;
    }
    
    .popover.bottom > .arrow::after {
        border-bottom-color: #000000;
    }
    
    .profile-card .profile-card-body .ui-avatar.circle:hover {
        box-shadow: 0 0 5px #FFFFFF;
    }
    
    .profile-card .profile-card-body .profile-card-name {
        color: #D0D0D0;
    }
    
    .profile-card .profile-card-body .profile-card-name:hover {
        color: #FFFFFF;
    }
    
    .profile-card .profile-card-body .profile-card-username {
        color: #A0A0A0;
    }
    
    .profile-card .profile-settings {
        color: #10A0FF;
        border-top-color: #696969;
    }
    
    .profile-card .profile-settings:hover {
        background-color: transparent;
        color: #10A0FF;
        text-shadow: 0 0 0.1em #10A0FF;
    }
    
    /* Last Change Status */
    .ui-status-lastchange {
        color: #868686;
    }
    
    /* Community Buttons */
    .community-button {
        color: #868686;
    }
    
    .community-button:hover,
    .community-button:focus,
    .ui-notification.dropdown.open .community-button {
        background-color: transparent;
        color: #FFFFFF;
    }
    
    .ui-notification .notification-menu-item:hover,
    .ui-notification .notification-menu-item:hover div,
    .ui-notification .notification-menu-item:focus,
    .ui-notification .notification-menu-item:focus div {
        background-color: transparent;
        color: #FFFFFF !important;
    }
    
    /* Comments */
    .ui-comment-app .open-comments {
        background-color: transparent;
    }
    
    .ui-comment-app .open-comments .btn.ui-open-comments,
    .ui-comment-app .open-comments .btn.ui-open-comments:focus:not(:hover),
    .ui-comment-app .open-comments .btn.ui-open-comments.open,
    .ui-comment-app .open-comments .btn.ui-open-comments.open:focus:not(:hover) {
        background-color: transparent;
        color: #868686;
        border-color: transparent;
    }
    
    .ui-comment-app .open-comments .btn.ui-open-comments:hover,
    .ui-comment-app .open-comments .btn.ui-open-comments.open:hover {
        background-color: transparent;
        color: #FFFFFF;
        border-color: transparent;
    }
    
    .ui-comment-app .open-comments .comment-settings {
        color: #868686;
    }
    
    .ui-comment-app .open-comments .comment-settings:hover {
        color: #FFFFFF;
    }
    
    .ui-comment-container .ui-no-comments div {
        color: #868686;
    }
    
    .ui-comment-button-container:not(.active):hover,
    .ui-comment-button-container.comment.active:not(.simple) {
        background-color: transparent;
    }
    
    .ui-comment-button-container .divider {
        border-color: #696969;
    }
    
    .ui-comment-container {
        background-color: #000000;
        border: 1px solid #696969;
    }
    
    .ui-comment-container:hover {
        background-color: #000000;
    }
    
    .ui-comment-container .ui-comments-container .ui-comment .comment-author {
        color: #D0D0D0;
    }
    
    .ui-comment-container .ui-comments-container .ui-comment .timestamp {
        color: #868686;
    }
    
    .ui-comment-container .ui-comments-container .ui-comment .comment-content {
        color: #FFFFFF;
    }
    
    .ui-comment-container .ui-comment-input-container .ui-comment-input-widgets .comment-textarea {
        background-color: #000000;
        color: #FFFFFF;
        border-color: #696969;
    }
    
    .ui-comment-container .ui-comment-input-container .ui-comment-input-widgets .comment-textarea::placeholder {
        color: #C5C5C5;
    }
    
    .ui-comment-container .ui-comment-input-container .ui-comment-input-widgets .btn-default {
        color: #D0D0D0;
        border-color: #696969;
    }
    
    .ui-comment-container .ui-comment-input-container .ui-comment-input-widgets .btn-default:hover {
        background-color: transparent;
        color: #FFFFFF;
        border-color: #696969;
    }
    
    /* Summary (Book Mode) */
    .summary {
        background-color: #1E1E1E;
        border-color: #696969;
    }
    
    .ui-summary-action {
        color: #C5C5C5;
    }
    
    .ui-summary-action:hover, .ui-summary-action:focus {
        color: #FFFFFF;
        text-shadow: 0 0 0.1em #FFFFFF;
    }
    
    .summary h1, .summary h2, .summary h3,
    .summary h4, .summary h5, .summary h6,
    .summary h1 .fa-angle-down,
    .summary h2 .fa-angle-down,
    .summary h3 .fa-angle-down,
    .summary h4 .fa-angle-down,
    .summary h5 .fa-angle-down,
    .summary h6 .fa-angle-down {
        color: #C5C5C5;
    }
    
    .summary .toolbar,
    .summary h1.collapsible:not(:first-child),
    .summary h2.collapsible:not(:first-child),
    .summary h3.collapsible:not(:first-child),
    .summary h4.collapsible:not(:first-child),
    .summary h5.collapsible:not(:first-child),
    .summary h6.collapsible:not(:first-child) {
        background-color: transparent;
        border-color: #696969;
    }
    
    .summary h1 + .nav-pills, .summary h2 + .nav-pills,
    .summary h3 + .nav-pills, .summary h4 + .nav-pills,
    .summary h5 + .nav-pills, .summary h6 + .nav-pills {
        padding-left: 0;
        padding-right: 48px;
    }
    
    .summary .nav-pills > li > a,
    .summary .nav-pills > li > a:visited {
        color: #D0D0D0;
        padding-left: 30px;
        border-left: 2px solid transparent;
    }
    
    .summary .nav-pills > li > a:hover,
    .summary .nav-pills > li > a:focus,
    .summary .nav-pills > li.active > a,
    .summary .nav-pills > li.active > a:hover,
    .summary .nav-pills > li.active > a:focus {
        color: #EEEEEE;
        text-decoration: none;
        border-left-color: #EEEEEE;
    }
    
    /* Table of Content */
    .ui-toc-dropdown .nav > li > a {
        color: #868686;
    }
    
    .ui-toc-dropdown .nav > .active:focus > a,
    .ui-toc-dropdown .nav > .active:hover > a,
    .ui-toc-dropdown .nav > .active > a,
    .ui-toc-dropdown .nav > li > a:focus,
    .ui-toc-dropdown .nav > li > a:hover {
        color: #EEEEEE;
        border-left-color: #EEEEEE;
    }
    
    .expand-toggle, .back-to-top, .go-to-bottom {
        color: #868686;
    }
    
    .expand-toggle:hover, .expand-toggle:focus,
    .back-to-top:hover, .back-to-top:focus,
    .go-to-bottom:hover, .go-to-bottom:focus {
        color: #EEEEEE;
    }
    
    /* Links */
    .markdown-body a {
        color: #10A0FF;
    }
    
    .markdown-body a:hover {
        text-decoration: none;
        text-shadow: 0 0 0.1px #10A0FF;
    }
    
    /* Marks */
    .markdown-body mark {
        background-color: transparent;
        color: inherit;
        padding: 0;
        border-bottom: 1px solid #E8A635;
    }
    
    /* Split Lines */
    .markdown-body hr {
        height: 1px;
        color: #EEEEEE;
    }
    
    /* Headers */
    .markdown-body h1,
    .markdown-body h2,
    .markdown-body h3,
    .markdown-body h4,
    .markdown-body h5,
    .markdown-body h6 {
        color: #F5DEB3;
        border-color: #F5DEB3;
    }
    
    .markdown-body h1 .octicon-link,
    .markdown-body h2 .octicon-link,
    .markdown-body h3 .octicon-link,
    .markdown-body h4 .octicon-link,
    .markdown-body h5 .octicon-link,
    .markdown-body h6 .octicon-link {
        color: #C5C5C5;
        text-shadow: none;
    }
    
    /* Images */
    .markdown-body img {
        background-color: transparent;
    }
    
    /* Quote Blocks */
    .markdown-body blockquote {
        color: #FFFFFF;
        border-color: #C5C5C5;
    }
    
    .markdown-body blockquote small {
        color: #C5C5C5;
    }
    
    .markdown-body blockquote small > .fa-user {
        color: #638FAC;
    }
    
    .markdown-body blockquote small > .fa-clock-o {
        color: #689F7A;
    }
    
    /* Information */
    .markdown-body div.alert-info {
        background-color: #1F3742;
        color: #BCE8F1;
    }
    
    /* Spoilers */
    .markdown-body details {
        background-color: #0A0A0A;
        color: #EEEEEE;
        padding-left: 10px;
        padding-right: 10px;
        border: none;
        border-radius: 3px;
        margin-bottom: 16px;
        overflow: auto; /* Avoid the margin collapsing. */
    }
    
    .markdown-body details > summary {
        color: #D0D0D0;
    }
    
    .markdown-body details > :not(summary):first-child,
    .markdown-body details > summary + * {
        margin-top: 5px;
    }
    
    .markdown-body details > :last-child {
        margin-bottom: 10px;
    }
    
    /* Difinition Lists */
    .markdown-body dl dt {
        font-style: normal;
        margin-bottom: 8px;
    }
    
    /* Tables */
    .markdown-body table {
        width: fit-content;
        max-width: 100%;
        margin-left: auto;
        margin-right: auto;
    }
    
    .markdown-body table thead tr {
        background-color: #000000;
    }
    
    .markdown-body table tr {
        background-color: #1E1E1E;
    }
    
    .markdown-body table tr:nth-child(2n) {
        background-color: #0A0A0A;
    }
    
    /* Codes */
    .markdown-body code, .markdown-body pre {
        background-color: #282C34;
        color: #ABB2BF;
    }
    
    .markdown-body code {
        padding-bottom: .1em;
    }
    
    .markdown-body code,
    .markdown-body pre,
    .markdown-body kbd,
    .markdown-body samp {
        font-family: "JetBrains Mono", Menlo, Monaco, Consolas, "Courier New", monospace;
        font-variant-ligatures: none;
    }
    
    .markdown-body pre code .gutter.linenumber {
        border-right-color: #555555 !important;
    }
    
    .markdown-body .token.directive-hash {
        color: #C678DD;
        font-style: italic;
    }
    
    .markdown-body .token.keyword {
        color: #C678DD;
        font-style: italic;
    }
    
    .markdown-body .token.namespace {
        color: #56B6C2;
        opacity: 1;
        font-style: italic;
    }
    
    .markdown-body .token.type {
        color: #E5C07B;
    }
    
    .markdown-body .token.function {
        color: #61AFEF;
    }
    
    .markdown-body .token.param {
        color: #D19A66;
    }
    
    .markdown-body .token.gvariable,
    .markdown-body .token.macro,
    .markdown-body .token.property {
        color: #E06C75;
    }
    
    .markdown-body .token.string,
    .markdown-body .token.char {
        color: #98C379;
    }
    
    .markdown-body .token.string .token.esc,
    .markdown-body .token.char .token.esc {
        color: #56B6C2;
    }
    
    .markdown-body .token.number {
        color: #00B66C;
    }
    
    .markdown-body .token.boolean {
        color: #C678DD;
        font-style: italic;
    }
    
    .markdown-body .token.operator,
    .markdown-body .token.punctuation {
        background-color: transparent;
        color: #ABB2BF;
    }
    
    .markdown-body .token.comment {
        color: #6C80A3;
        font-style: italic;
    }
    
    .markdown-body .hljs-tag {
        color: #ABB2BF;
    }
    
    .markdown-body .hljs-name {
        color: #E06C75;
    }
    
    .markdown-body .hljs-attr {
        color: #D19A66;
    }
    
    .markdown-body .hljs-string {
        color: #98C379;
    }
    
    /* Icons */
    .markdown-body .lmn-icon {
        font-family: "FontAwesome";
    }
    
    /* Version Annotations */
    .markdown-body .lmn-va {
        color: #72FF72;
        font-size: .75em;
    }
    
    .markdown-body .lmn-vs {
        border-bottom: 1px solid #72FF72;
    }
    
    .markdown-body .lmn-vs::before, .markdown-body .lmn-vs::after {
        letter-spacing: -.2em;
        content: "\00A0";
    }
    
    /* Ko-fi */
    .markdown-body .lmn-kofi:hover {
        box-shadow: 0 0 5px #17BEE5;
    }
    
    /* Theme License */
    #lmn-dark-theme-license {
        color: #C5C5C5;
        font-size: 14px;
        padding-top: 2px;
        padding-bottom:2px;
    }
    
    #lmn-dark-theme-license > summary {
        font-size: 12px;
        padding: 0;
    }
</style>

<details id="lmn-dark-theme-license">
<summary>
Dark Theme License
</summary>

The MIT License (MIT)

Copyright (c) 2022 Luminous-Coder

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
</details>