<script src="https://cdnjs.cloudflare.com/ajax/libs/jszip/3.10.1/jszip.min.js"></script>
<script>
function exportToZip(data) {
	try {
		const parsed = typeof data === "string" ? JSON.parse(data) : data;
		const zip = new JSZip();
		for (const file of parsed.files) {
			const binary = atob(file.b64);
			const bytes = new Uint8Array(binary.length);
			for (let i = 0; i < binary.length; i++) {
				bytes[i] = binary.charCodeAt(i);
			}
			zip.file(file.name, bytes);
		}
		zip.generateAsync({ type: "blob" }).then(blob => {
			const url = URL.createObjectURL(blob);
			const a = document.createElement('a');
			a.href = url;
			a.download = "gumdrop_export.zip";
			document.body.appendChild(a);
			a.click();
			a.remove();
			URL.revokeObjectURL(url);
		});
	} catch (err) {
		console.error("JS exportToZip failed:", err);
	}
}
</script>