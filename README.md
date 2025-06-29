html_content = """
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form Input Data Bank</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            max-width: 600px;
            margin: 40px auto;
            background-color: #f7f7f7;
            padding: 20px;
            border-radius: 12px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        h2 {
            text-align: center;
        }
        label {
            display: block;
            margin-top: 15px;
            font-weight: bold;
        }
        input, select, textarea, button {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
            border-radius: 8px;
            border: 1px solid #ccc;
            box-sizing: border-box;
        }
        button {
            background-color: #007bff;
            color: white;
            font-size: 16px;
            margin-top: 20px;
            cursor: pointer;
            transition: 0.3s;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <h2>Form Input Data Bank</h2>
    <form method="POST" action="PASTE_GOOGLE_SCRIPT_URL_HERE">
        <label>Nama Bank:</label>
        <input type="text" name="Nama Bank" required>

        <label>Kode Bank:</label>
        <input type="text" name="Kode Bank" required>

        <label>No. Rekening:</label>
        <input type="text" name="No. Rekening" required>

        <label>Nama Pemilik:</label>
        <input type="text" name="Nama Pemilik" required>

        <label>Jenis Rekening:</label>
        <input type="text" name="Jenis Rekening" required>

        <label>Cabang/Wilayah:</label>
        <input type="text" name="Cabang/Wilayah" required>

        <label>Status:</label>
        <select name="Status" required>
            <option value="Aktif">Aktif</option>
            <option value="Tidak Aktif">Tidak Aktif</option>
        </select>

        <label>Catatan Tambahan:</label>
        <textarea name="Catatan Tambahan" rows="3"></textarea>

        <button type="submit">Kirim</button>
    </form>
</body>
</html>
"""

file_path = "/mnt/data/form_input_data_bank.html"
with open(file_path, "w", encoding="utf-8") as f:
    f.write(html_content)

file_path
