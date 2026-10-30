# 🧠 JS Client-Side Reverse Engineering Archive

A curated collection of online tools, frameworks, and resources for JavaScript analysis, deobfuscation, formatting, AST exploration, and client-side protection research. This archive is useful for understanding how modern client-side JS is transformed, bundled, protected, and reverse engineered.

---

## 🔧 Deobfuscation & Analysis

### 🔗 WebCrack
https://webcrack.netlify.app/  
A web-based tool for analyzing and deobfuscating JavaScript code. Unpacks Webpack bundles, deobfuscates obfuscator.io patterns, and unminifies code automatically.

### 🔗 Deobfuscate
https://deobfuscate.io/  
Automatically simplifies obfuscated JavaScript using common static analysis techniques like string decoding, constant folding, and control-flow cleanup.

### 🔗 Relative Deobfuscator
https://deobfuscate.relative.im/  
Online JavaScript deobfuscator powered by Synchrony, focused on restoring readability of heavily obfuscated scripts and simplifying common protection patterns.

### 🔗 Synchrony
https://github.com/relative/synchrony  
Open-source CLI deobfuscator that reverses common obfuscation patterns, cleans control-flow flattening, restores string arrays, and cleans dead code.

### 🔗 JS Nice
http://www.jsnice.org/  
Statistical deobfuscation engine that restores meaningful variable names and infers types from minified or obfuscated code using machine learning over a large JS corpus.

### 🔗 de4js
https://lelinhtinh.github.io/de4js/  
Online JavaScript deobfuscator and unpacker supporting multiple common obfuscation patterns including Eval, Packer, Obfuscator.io, AAEncode, JJEncode, JSFuck, and more. Works entirely in the browser without server-side processing.

### 🔗 CyberChef
https://gchq.github.io/CyberChef/  
The "Swiss Army Knife" for data transformation. Highly useful in JS reverse engineering for Base64/Hex decoding, XOR operations, string extraction, beautifying, unescaping, and entropy calculations.

---

## 🗺️ Source Map Extraction & Bundle Reconstruction

### 🔗 unwebpack-sourcemap
https://github.com/rare-freak/unwebpack-sourcemap  
CLI tool to extract and reconstruct the original, uncompiled source code directory tree directly from exposed Webpack source maps (`.map` files or embedded inline base64).

### 🔗 shuji
https://github.com/paazmaya/shuji  
Node.js utility to reverse engineer source maps into the original directory and file hierarchy.

### 🔗 sourcemapper
https://github.com/denandz/sourcemapper  
A fast Go tool that parses JavaScript source maps and extracts the original source tree from target endpoints.

### 🔗 SourceDetector
https://github.com/sunfishcode/SourceDetector  
Browser extension that monitors and automatically detects if a production website is leaking source map (`.js.map`) files during navigation.

---

## 🛡️ Obfuscation & Protection

### 🔗 Obfuscator.io
https://obfuscator.io/  
Popular JS obfuscation tool using control-flow flattening, string encoding, dead code injection, and identifier renaming.

### 🔗 JS-Confuser
https://js-confuser.com/  
Advanced obfuscation tool focused on heavily protecting JavaScript against reverse engineering with novel transformations and anti-tamper mechanisms.

### 🔗 JScrambler
https://jscrambler.com/  
Enterprise-grade JavaScript protection platform offering polymorphic obfuscation, runtime application self-protection (RASP), anti-debugging, and webpage integrity monitoring.

### 🔗 MeowShield
https://meowshield.com/  
JavaScript protection tool designed to prevent copying and analysis of client-side code.

### 🔗 PreEmptive Online JavaScript Obfuscator
https://www.preemptive.com/online-javascript-obfuscator/  
Online JavaScript obfuscation tool focused on protecting client-side code against reverse engineering, tampering, and debugging.

### 🔗 Google Closure Compiler
https://developers.google.com/closure/compiler  
Comprehensive compiler providing Advanced Optimization mode, which aggressively renames symbols, inlines functions, and removes unused code.

---

## 🎨 Formatting & Minification

### 🔗 Beautifier
https://beautifier.io/  
Fast online code formatter for JavaScript, HTML, and CSS (powered by `js-beautify`).

### 🔗 HTMLStrip Unminify JS
https://www.htmlstrip.com/unminify-javascript/  
Restores readability of minified or compressed JavaScript code.

### 🔗 UglifyJS Online
https://skalman.github.io/UglifyJS-online/  
Browser-based JS minifier using UglifyJS.

### 🔗 Terser Playground
https://try.terser.org/  
Online playground for testing JavaScript minification and compression with Terser.

### 🔗 Prettier Playground
https://prettier.io/playground/  
Opinionated code formatter playground for standardizing syntax and formatting complex JavaScript files.

---

## 🌳 AST & Code Analysis

### 🔗 AST Explorer
https://astexplorer.net/  
Interactive web app for parsing and visualizing Abstract Syntax Trees (AST) across dozens of JavaScript/TypeScript parsers (Babel, Acorn, Espree, SWC, Shift).

### 🔗 Babel REPL
https://babeljs.io/repl  
Real-time JS transpilation tool used to study AST-based transformations and Babel plugin behavior.

### 🔗 SWC Playground
https://play.swc.rs/  
Interactive playground for SWC (Rust-based extensible JavaScript/TypeScript compiler) to test AST transforms and high-performance minification.

### 🔗 Shift AST
https://shift-ast.org/  
Formal JavaScript AST specification and toolset designed specifically for static analysis, pattern matching, and automated transformations.

### 🔗 Source Map Explorer
https://github.com/danvk/source-map-explorer  
Visualizes JavaScript bundles using source maps to show which files and dependencies contribute to final bundle size. Useful for analyzing webpack/Vite builds and inspecting bundled modules.

---

## 🔬 Dynamic Analysis, Hooking & Interception

### 🔗 JStillery
https://mindedsecurity.github.io/jstillery/  
Advanced JavaScript deobfuscation via partial evaluation. Combines AST analysis with selective code execution to resolve complex string concatenation, unpack packed code, and simplify control flow.

### 🔗 Requestly
https://requestly.com/  
Browser extension and desktop app that allows intercepting and redirecting network requests. Enables swapping remote production scripts with local or beautified/instrumented copies on the fly without proxy configuration.

### 🔗 Tampermonkey / Violentmonkey
https://www.tampermonkey.net/  
Userscript managers enabling runtime script injection, API monkey-patching, prototype hooking (e.g. `Function.prototype.toString`, `eval`, `Proxy`), and anti-debugging bypasses (`debugger;` statement suppression).

### 🔗 Ajax-Hook / XHook
https://github.com/wendux/Ajax-hook  
Client-side interceptors for `XMLHttpRequest` and `fetch` calls, enabling dynamic monitoring and modification of API requests and responses directly in the browser runtime.

---

## 🕵️ Browser Fingerprinting & Anti-Bot Research

### 🔗 BrowserLeaks
https://browserleaks.com/  
Comprehensive suite of web browser security and privacy testing tools covering Canvas, WebGL, AudioContext, Font, WebRTC, Client Hints, and TLS/JA3 fingerprinting.

### 🔗 CreepJS
https://abrahamjuliot.github.io/creepjs/  
Advanced browser fingerprinting and anomaly detection tool. Tests prototype tampering, proxy object detection, headless browser cues, and anti-detect evasion mechanisms.

### 🔗 AmIUnique
https://amiunique.org/  
Research platform that calculates how unique and trackable a browser configuration is through canvas, headers, plugins, and rendering hardware.

### 🔗 Fingerprint.com Demo
https://fingerprint.com/products/fingerprint-pro/  
Interactive demo of modern commercial device and browser fingerprinting algorithms.

---

## 🔏 Esoteric & Exotic Encoders

### 🔗 JSFuck
http://www.jsfuck.com/  
Esoteric programming technique that executes arbitrary JavaScript using only 6 distinct characters: `[ ] ( ) ! +`. Widely analyzed in WAF evasion and payload obfuscation research.

### 🔗 AAEncode & JJEncode
https://utf-8.jp/public/aaencode.html  
Classic Japanese emoticon and Japanese quote encoders that transform JavaScript code into valid ASCII-art style expressions.

---

## 📚 Essential Guides & AST References

### 🔗 Babel Plugin Handbook
https://github.com/jamiebuilds/babel-handbook  
Comprehensive guide on writing custom Babel plugins and traversing/manipulating JavaScript ASTs. Essential for authoring custom deobfuscators.

### 🔗 JavaScript Deobfuscation Guide (Relative)
https://relative.im/blog  
Technical deep-dives into modern obfuscation patterns (control flow flattening, proxy functions, string array encodings) and automated reversal techniques.

---

## 💡 Notes

This archive is useful for:
- Reverse engineering client-side JavaScript
- Understanding obfuscation & anti-tamper techniques
- Learning AST-based transformations and building custom deobfuscators
- Bypassing client-side anti-debugging and anti-analysis checks
- Investigating browser fingerprinting and bot detection mechanisms
- Reconstructing original source code from exposed source maps
