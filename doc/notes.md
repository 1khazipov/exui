// Inside your Chat class constructor
this.fileInput = document.createElement("input");
this.fileInput.type = "file";
this.fileInput.style.display = "none";
this.fileInput.addEventListener("change", (event) => this.handleFileUpload(event));

this.uploadButton = new controls.Button("📎 Upload File", () => { this.fileInput.click() }, "upload-button");
panel.appendChild(this.uploadButton.element);
panel.appendChild(this.fileInput);
