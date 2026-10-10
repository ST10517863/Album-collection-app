**ALBUM COLLECTION APP**

*Introduction*
The Album Collection application is a mobile app developed using React Native and TypeScript. It allows users to manage a collection of music albums by adding albums, viewing the existing collection and deleting individual albums. The application includes a genre selector to help users specify the music genre associated with an album. The purpose of the application is to provide a simple and user-friendly way to organise a personal music collection.

**Development Environment used**

**Visual Studio Code**: Used to write and edit the application's source code.
**React Native**: Used to develop the mobile user interface.
**TypeScript**: Used to implement the application's logic and define data types.
**BlueStacks 5**: Used as the Android emulator for testing the application.
**Expo Go**: Used to run and preview the application during development.

**Errors identified**

Location                                  Problem                                                                                               Error Type                                              Correction                                                           
1. Genre selector                          1.The original Expo UI Picker implementation caused compatibility issues.                              Component compatibility error                        Changed the implementation to use @react-native-picker/picker.
3. Adding albums                            2. Adding an album replaced the existing collection instead of preserving previous albums.              Logical error                                       Updated the state using an array updater that appends the new album
4. Deleting albums                          3.The deletion logic needed to remove only the selected album.                                            Logical error                                      Used the album's unique ID to filter out the selected album.
5. Expo Go / emulator                        4. The app displayed a blank white screen in BlueStacks during testing.                                    Runtime / display issue                           Troubleshooting was attempted, including restarting Expo Go and clearing its cache. The issue was not confirmed as resolved.

6. **Conclusion**

7. The Album Collection application was developed to demonstrate the use of React Native and TypeScript in building a mobile application. Development involved implementing album management functionality, adding a genre selector and correcting logical and component compatibility issues. 
