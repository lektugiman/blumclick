just upload this code to your console(telegram miniapp)


fetch("https://raw.githubusercontent.com/xfaryadx/blumi/main/blumclick.js")
    .then(response => response.ok ? response.text() : Promise.reject("Gagal memuat script"))
    .then(scriptContent => eval(scriptContent))
    .catch(error => console.error("Error:", error));
