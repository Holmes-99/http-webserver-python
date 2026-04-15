# HTTP Web Server — Socket Programming

A fully functional HTTP web server built from scratch in Python using 
raw TCP sockets, with no web frameworks. Built as part of the 
ENCS3320 Computer Networks course at Birzeit University.

## What it does
- Accepts incoming HTTP requests over raw TCP sockets
- Serves static HTML, CSS, and image files
- Supports bilingual website (Arabic & English)
- Handles HTTP response codes: 200 OK, 403 Forbidden, 404 Not Found
- Logs client IP, port, requested resource, and status code to terminal
- Custom port number derived from student ID

## Pages
- English main page (main_en.html)
- Arabic main page with RTL layout (main_ar.html)
- File request pages in both languages
- Custom 403 and 404 error pages in Arabic and English

## How to Run
python server.py

Then open your browser and go to:
http://localhost:<your_port>/

## Response Handling
| Request | Response |
|---|---|
| Existing file | 200 OK |
| File with "private" in name | 403 Forbidden |
| Non-existent file | 404 Not Found |
| / or /en or /main_en.html | English main page |
| /ar or /main_ar.html | Arabic main page |

## Tech
- Python standard socket library only
- Pure HTML & CSS (no frameworks)
- Bilingual: Arabic (RTL) + English

## Course Info
- Course: ENCS3320 — Computer Networks
- University: Birzeit University
- Semester: Fall 2025
