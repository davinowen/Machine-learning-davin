import os

for week in range(2, 15):
    folder_name = f"Week-{week:02d}"
    os.makedirs(folder_name, exist_ok=True)
    # Membuat file kosong agar folder terdeteksi Git
    with open(os.path.join(folder_name, ".gitkeep"), "w") as f:
        pass
print("Folder Week-02 sampai Week-14 berhasil dibuat!")