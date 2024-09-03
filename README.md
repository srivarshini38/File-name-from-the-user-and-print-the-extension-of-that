# File-name-from-the-user-and-print-the-extension-of-that
def print_file_extension():
    filename = input("Input the Filename: ")
    extension = filename.split(".")[-1]
    
    # Mapping of common extensions to their file types
    extensions_map = {
        "py": "python",
        "txt": "text",
        "doc": "document",
        "docx": "document",
        "jpg": "image",
        "jpeg": "image",
        "png": "image",
        "pdf": "PDF",
        "html": "HTML"
        # Add more mappings as needed
    }
    
    file_type = extensions_map.get(extension, "unknown")
    print(f"The extension of the file is: '{file_type}'")

print_file_extension()
