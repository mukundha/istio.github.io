---
title: Search Results
url: /search.html
sidebar_none: true
---

<style>
    .gs-webResult div.gs-visibleUrl-long, .gs-promotion div.gs-visibleUrl-long {
        padding-bottom: 0;
    }

    table, th, td, tr {
        border: 0;
        padding: 0;
    }

    table {
        margin-left: .5em;
        margin-right: 0;
    }

    table p:first-of-type {
        margin-top: 0;
    }

    table p:last-of-type {
        margin-bottom: 0
    }

    tr.oneof>td {
        border: 0;
    }

    table {
        border-collapse: collapse;
        border-spacing: 0;
    }

    tr:first-child th:first-child {
        border: 0;
    }

    tr:first-child td:first-child {
        border: 0;
    }

    tr:first-child th:last-child {
        border: 0;
    }

    tr:first-child td:last-child {
        border: 0;
    }

    tr:last-child td {
        border: 0;
    }

    tr:last-child td:first-child {
        border: 0;
    }

    tr:last-child td:last-child {
        border: 0;
    }

    tr th:last-child {
        border: 0;
    }

    tr td:last-child {
        border: 0;
    }
</style>

<div class="search-results">
    <script>
        (function() {
            var cx = '{{< search_engine_id >}}';
            var gcse = document.createElement('script');
            gcse.type = 'text/javascript';
            gcse.async = true;
            gcse.src = 'https://cse.google.com/cse.js?cx=' + cx;
            var s = document.getElementsByTagName('script')[0];
            s.parentNode.insertBefore(gcse, s);
        })();
    </script>

    <gcse:searchresults-only></gcse:searchresults-only>
</div>

<script>
    function getParameterByName(name, url) {
        if (!url) url = window.location.href;
        name = name.replace(/[\[\]]/g, "\\$&");
        var regex = new RegExp("[?&]" + name + "(=([^&#]*)|&|#|$)"),
            results = regex.exec(url);
        if (!results) return null;
        if (!results[2]) return '';
        return decodeURIComponent(results[2].replace(/\+/g, " "));
    }
    var q = getParameterByName('q', window.location.href);
    document.getElementsByName('q')[0].value = q;
</script>
