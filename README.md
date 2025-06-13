## How to Compile

1. Open a terminal or command prompt.  
2. Navigate to the project directory.  
3. Compile the code using:

    g++ -std=c++17 -I. main.cpp MainWindow.cpp StorageManager.cpp StoredItem.cpp -o StorageGUI `pkg-config --cflags --libs Qt5Widgets`

## How to Run

- On Linux or macOS:  
    ./StorageGUI

- On Windows:  
    StorageGUI.exe

## How to Use

1. Launch the program.  
2. The Qt window will appear with controls:  
3. Input fields for **ID**, **Description**, **Location** and an **Add Item** button  
4. A **Find by ID** field and button to display an item's details  
5. A **Remove by ID** field and button to delete an item  
6. A list widget showing all items sorted by description  
7. Use **File > Exit** to close the application  

You interact by typing into the matching field and clicking its button. The program checks for errors like:

Trying to add an item with a duplicate ID

Finding or removing an item that doesn’t exist

Listing when no items have been added
