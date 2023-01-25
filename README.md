This script is for sorting files in selected folder by file types.
    !!!!ATTENTION: Don't use this script for programm folders!!!!!!

    Files in subfolders are also sorted.
    In selected folder are created 5 folders(images, video, documents, audio, archives)
    Depending on the type, the file is moved to one of the following folders:
        'images': ['JPEG', 'PNG', 'JPG', 'SVG'],
        'video': ['AVI', 'MP4', 'MOV', 'MKV'],
        'documents': ['DOC', 'DOCX', 'TXT', 'PDF', 'XLSX', 'PPTX', 'XLS', 'CSV'],
        'audio': ['MP3', 'OGG', 'WAV', 'AMR'],
        'archives': ['ZIP', 'GZ', 'TAR']
    Files with a type not listed above are not moved.
    Unpacked archives replaced into folder "archives" in folder with archives name 
    Also, name all files and folders are normalized (transliterate cyrillik symbols into latin, 
                                                    all symbols except latin and digit are replaced by "_" )
    Empty folders are deleted
    
    
    how to use:
    copy file on your computer.
    run the script in cmd, and enter the path to folder as comand argument.
    example for Windows:
      C:\Users\username\Desktop\Scripts>python sort_file_in_folder.py C:\Users\username\Desktop\unsorted\er2
