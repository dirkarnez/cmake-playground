cmake_minimum_required(VERSION 3.14)

project(cmake-playground)

file(DOWNLOAD "https://github.com/dirkarnez/pugixml-prebuilt/releases/download/v1.12.1/pugixml-v1.12.1-x86_64-posix-seh-rev0-8.1.0.zip" "$ENV{TEMP}/${PROJECT_NAME}/downloads/pugixml-v1.12.1-x86_64-posix-seh-rev0-8.1.0.zip")

# "external" is in "build" folder
file(ARCHIVE_EXTRACT INPUT "$ENV{TEMP}/${PROJECT_NAME}/downloads/pugixml-v1.12.1-x86_64-posix-seh-rev0-8.1.0.zip" DESTINATION "./external/pugixml-v1.12.1-x86_64-posix-seh-rev0-8.1.0")