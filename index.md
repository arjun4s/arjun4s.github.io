---
layout: page2
title: Halo, Dunia!
tagline: 
---
{% include JB/setup %}
## Selamat Datang
Terima kasih atas kunjungan kamu di Kodeloka.

## Arsip Posting
<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>


		<h2>Permainan Favorit</h2>
		<ul>
			<li><a onclick='window.dvminesweeper['iframe']()'><img alt='Minesweeper' src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAAhUlEQVQ4jZ2TYQpAIQiDPfqOtpvt/TLMVOQJUVTfmkpmQwDQdD4GAEnSb5FOoBUEcF2uBACIpMxMD0zyAA6TFMmzF+DXRRTJsM8tnG1XcBCoc8+wr80sv347cXBh+4yr4NFBU6xp1IVMOc9QjAXci0w5x9xLkabPVev6dhbK3eX151oV7gN7/S8cyxYRWAAAAABJRU5ErkJggg==' style='width: 32px; height: 32px;' title='Minesweeper'/></a></li>
			<li><a onclick='window.dvpinball['iframe']()'><img alt='Pinball' src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAAfklEQVQ4jZWSyw3AMAxCGT2rMRm9tJVLiJMi+RKZ51+AoDGGUqTcaEwi2YOqsSbXICmSAqBoduOdKABpHE0Ar9RBXoBXJzmNUiG2C03VXQnwAaf2dx20gG4Hz/sWkK7g5i2gGjyOz7gyR0A94y9z0XKE5Q9MkPRtbaFHUoioC3+TBCKVpEkJAAAAAElFTkSuQmCC' style='width: 32px; height: 32px;' title='Pinball'/></a></li>
			<li><a onclick='window.dvsolitaire['iframe']()'><img alt='Solitaire' src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAAZ0lEQVQ4je2SQQrAIAwEF5Q+2+7T8jN7sTaiSS7iqYE9BJyRaIBFkaxWVucnWETMAPAl3u2hgGT1qsGx4MY1gG+/RdAecpboOa2on/AFOZUO5VR6b8JaoiGdX3Ba4O1BKMC3rlaGegANmnZ42h6lmwAAAABJRU5ErkJggg==' style='width: 32px; height: 32px;' title='Solitaire'/></a></li>
		</ul>
<script>
        (function(){
            let winbox;
            window.dvminesweeper = {
                "iframe": function(){
                    new WinBox("Minesweeper", {
                        url: "https://arjun4s.github.io/sow98/programs/minesweeper/index.html",
                        class: "iframe"
                    });
                },
            };
            window.dvpinball = {
                "iframe": function(){
                    new WinBox("Pinball", {
                        url: "https://arjun4s.github.io/sow98/programs/pinball/space-cadet.html",
                        class: "iframe"
                    });
                },
            };
            window.dvsolitaire = {
                "iframe": function(){
                    new WinBox("Solitaire", {
                        url: "https://arjun4s.github.io/sow98/programs/js-solitaire/index.html",
                        class: "iframe"
                    });
                },
            };
            window.buttons = {
                minimize: function(){
                    winbox.minimize();
                },
                maximize: function(){
                    winbox.maximize();
                },
                fullscreen: function(){
                    winbox.fullscreen();
                },
                center: function(){
                    winbox.move("center", "center");
                },
                move: function(){
                    winbox.move("right", "bottom");
                },
                resize: function(){
                    winbox.resize("50%", "50%");
                },
                title: function(){
                    winbox.setTitle("Title-" + Math.random());
                },
                color: function(){
                    winbox.setBackground(
                        "rgb(" + (Math.random() * 255 | 0) + "," +
                                 (Math.random() * 255 | 0) + "," +
                                 (Math.random() * 255 | 0) + ")"
                    );
                },
                modal: function(){
                    winbox.body.parentNode.classList.toggle("modal");
                },
                add: function(){
                    winbox.addClass("my-theme");
                },
                remove: function(){
                    winbox.removeClass("my-theme");
                },
                close: function(){
                    winbox.close();
                },
                force_close: function () {
                    winbox.close(true);
                }
            };
        }());
</script>
