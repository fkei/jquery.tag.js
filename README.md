#jquery.tag.js

## Function
### Add a tag element.

$.tag = function(name, options){ ... }


before:

    <div id="hoge">Test</div>

script:

    $("#hoge")
        .tag("a", {"href": "http://example.com/", id: "home", class: "foo bar"})
            .tag("span").text("goto home").gat()
        .gat()
    ;

after:

    <div id="hoge">
        <a href="http://example.com/" id="home", class="foo bar">
            <span>goto home</span>
        </a>
    </div>
    
### Add new tag element.

$.tagset = function(name, options) { ... }


before:

    <div id="hoge">Test</div>

script:

    $("#hoge")
        .tag("a", {"href": "http://example.com/", id: "home", class: "foo bar"})
            .tag("span").text("goto home").gat()
        .gat()
    ;


after:

    <div id="hoge">
        <a href="http://example.com/" id="home", class="foo bar">
            <span>goto home</span>
        </a>
    </div>


### Add a javascript.

$.next = function() { ... }
script:

    $("#hoge")
        .tag("a", {"href": "http://example.com/", id: "home", class: "foo bar"}).gat()
        .next(function() {
            alert("ALERT");
        })
    ;


### Close the element tag.

$.gat = function() { ... }






