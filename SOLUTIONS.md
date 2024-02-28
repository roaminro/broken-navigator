#1: 
    
    - search "logs" directory
    - open "navigator.log" file
    - Password: FLAG-Ezeg9cMX

#2:
    
    - open devtools
    - show hidden button "Load via Rust"
    - get coordinates: X:69091Y:45977Z:98163T:46510

#3:

    - open devtools
    - type `await window.__TAURI_INVOKE__("tauri",{__tauriModule:"Fs",message:{cmd:"writeFile",path: "navigation/active/Earth.cord", contents: [102, 108, 97, 103], options: { dir: 17 } } })`
    - (17 being `BaseDirectory.Resource` see https://github.com/tauri-apps/tauri/blob/e816a46b953092053d72c70feddf48a8c273c80d/tooling/api/src/fs.ts#L97)
    - check coordinates and get: FLAG-agVvrzmBFl