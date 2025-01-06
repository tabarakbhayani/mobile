<!DOCTYPE html>
<html lang="en">
<head>
    <!-- BEGIN LivePerson Monitor. -->
    <script type="text/javascript">
        window.lpTag = window.lpTag || {};
        if (typeof window.lpTag._tagCount === 'undefined') {
            window.lpTag = {
                wl: lpTag.wl || null,
                scp: lpTag.scp || null,
                site: '9994318' || '',
                section: lpTag.section || '',
                tagletSection: lpTag.tagletSection || null,
                autoStart: lpTag.autoStart !== !1,
                ovr: lpTag.ovr || {},
                _v: '1.10.0',
                _tagCount: 1,
                protocol: 'https:',
                events: {
                    bind: function (t, e, i) {
                        lpTag.defer(function () {
                            lpTag.events.bind(t, e, i)
                        }, 0)
                    },
                    trigger: function (t, e, i) {
                        lpTag.defer(function () {
                            lpTag.events.trigger(t, e, i)
                        }, 1)
                    }
                },
                defer: function (t, e) {
                    if (e === 0) {
                        this._defB = this._defB || [];
                        this._defB.push(t);
                    } else if (e === 1) {
                        this._defT = this._defT || [];
                        this._defT.push(t);
                    } else {
                        this._defL = this._defL || [];
                        this._defL.push(t);
                    }
                },
                load: function (t, e, i) {
                    var n = this;
                    setTimeout(function () {
                        n._load(t, e, i)
                    }, 0)
                },
                _load: function (t, e, i) {
                    var n = t;
                    if (!t) {
                        n = this.protocol + '//' + (this.ovr && this.ovr.domain ? this.ovr.domain : 'lptag.liveperson.net') + '/tag/tag.js?site=' + this.site;
                    }
                    var o = document.createElement('script');
                    o.setAttribute('charset', e ? e : 'UTF-8');
                    if (i) {
                        o.setAttribute('id', i);
                    }
                    o.setAttribute('src', n);
                    document.getElementsByTagName('head').item(0).appendChild(o);
                },
                init: function () {
                    this._timing = this._timing || {};
                    this._timing.start = (new Date).getTime();
                    var t = this;
                    if (window.attachEvent) {
                        window.attachEvent('onload', function () {
                            t._domReady('domReady')
                        });
                    } else {
                        window.addEventListener('DOMContentLoaded', function () {
                            t._domReady('contReady')
                        }, !1);
                        window.addEventListener('load', function () {
                            t._domReady('domReady')
                        }, !1);
                    }
                    if (typeof window._lptStop === 'undefined') {
                        this.load();
                    }
                },
                start: function () {
                    this.autoStart = !0;
                },
                _domReady: function (t) {
                    if (!this.isDom) {
                        this.isDom = !0;
                        this.events.trigger('LPT', 'DOM_READY', { t: t });
                    }
                    this._timing[t] = (new Date).getTime();
                },
                vars: lpTag.vars || [],
                dbs: lpTag.dbs || [],
                ctn: lpTag.ctn || [],
                sdes: lpTag.sdes || [],
                hooks: lpTag.hooks || [],
                identities: lpTag.identities || [],
                ev: lpTag.ev || []
            };
            lpTag.init();
        } else {
            window.lpTag._tagCount += 1;
        }
    </script>
    <!-- END LivePerson Monitor. -->
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Latest Phones</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 800px;
            margin: auto;
            background: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .phone {
            border-bottom: 1px solid #ccc;
            padding: 10px 0;
        }
        .phone:last-child {
            border-bottom: none;
        }
        .phone h2 {
            margin: 0;
        }
        .phone p {
            margin: 5px 0;
        }
        .phone ul {
            padding-left: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="phone">
            <h2>Apple iPhone 14 Pro</h2>
            <p><strong>Release Date:</strong> September 2024</p>
            <p><strong>Features:</strong></p>
            <ul>
                <li>6.1-inch Super Retina XDR display</li>
                <li>A18 Bionic chip</li>
                <li>Pro camera system with 48MP main camera</li>
                <li>5G capable</li>
                <li>Face ID</li>
            </ul>
        </div>
        <div class="phone">
            <h2>Samsung Galaxy S24 Ultra</h2>
            <p><strong>Release Date:</strong> January 2025</p>
            <p><strong>Features:</strong></p>
            <ul>
                <li>6.8-inch Dynamic AMOLED 2X display</li>
                <li>Exynos 2200/Snapdragon 895 processor</li>
                <li>Quad camera setup with 108MP main sensor</li>
                <li>5G capable</li>
                <li>In-display fingerprint sensor</li>
            </ul>
        </div>
    </div>
</body>
</html>
