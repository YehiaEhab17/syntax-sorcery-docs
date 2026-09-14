

Piston API

Free hosted instance at [https://emkc.org/api/v2/piston/runtimes](https://emkc.org/api/v2/piston/runtimes)

supports 60+ languages including Python, Java, JavaScript, Rust, C, C++, Go, etc.

Simple REST POST: send code + language + stdin, get stdout back

integration: fetch("[https://emkc.org/api/v2/piston/execute](https://emkc.org/api/v2/piston/execute)", { body: {language, version, files: [{content: code}]}, … })

Can also self-host (needs deciding)

monaco editor (the vscode editor) for users to input their code
