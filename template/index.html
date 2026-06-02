from PIL import Image
from PIL.ExifTags import TAGS
import tkinter as tk
from tkinter import filedialog, scrolledtext

def open_image():
    filepath = filedialog.askopenfilename(
        filetypes=[("Image Files", "*.jpg *.jpeg *.png *.tiff")]
    )

    if not filepath:
        return

    result.delete(1.0, tk.END)

    try:
        image = Image.open(filepath)
        exif_data = image.getexif()

        if not exif_data:
            result.insert(tk.END, "No EXIF metadata found.")
            return

        for tag_id, value in exif_data.items():
            tag = TAGS.get(tag_id, tag_id)
            result.insert(tk.END, f"{tag}: {value}\n")

    except Exception as e:
        result.insert(tk.END, f"Error: {e}")

root = tk.Tk()
root.title("Simple EXIF Viewer")
root.geometry("700x500")

btn = tk.Button(root, text="Open Image", command=open_image)
btn.pack(pady=10)

result = scrolledtext.ScrolledText(root)
result.pack(fill=tk.BOTH, expand=True)

root.mainloop()
