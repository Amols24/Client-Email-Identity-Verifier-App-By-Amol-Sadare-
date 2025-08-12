# Client-Email-Identity-Verifier-App-By-Amol-Sadare-

In my journey to master Python with practical, real-world applications, I recently built a desktop-based utility called the Client Email Identity Verifier App. This tool simulates the core logic behind email-based user verification systems — the kind of functionality we often see in user onboarding, secure logins, and password recovery flows.

The app offers a simple and intuitive GUI built using Python’s Tkinter library. When a user runs the .exe, they are greeted with a clean interface prompting them to enter their email address. Once submitted, the application generates a secure 6-digit One-Time Password (OTP) and sends it to the provided email via Gmail’s SMTP service using an App Password for added security.

A key part of the app is the OTP verification workflow. After the OTP is sent, the user is prompted to enter it. The app then compares the input with the original OTP and gives immediate feedback on whether the verification was successful or not. To maintain responsible use and mimic real-world rate limiting, I added a session-based cap of four OTP send attempts. After reaching the limit, the user must close and reopen the app to request more OTPs. This logic adds a subtle touch of anti-spam protection and user discipline.

Once the app is built and tested, I packaged it into a standalone .exe using PyInstaller, so users can run it without having Python installed. As a final touch, I included a clickable LinkedIn profile link within the app so that clients or users can verify the developer identity behind the tool — a small detail to demonstrate transparency and ownership.

This project taught me not just about GUI design and email integration, but also about user flow, session logic, and deployment. It mirrors a critical part of many authentication systems and serves as a strong foundational base for building more advanced ID verification tools in the future — including SMS-based OTP, token-based APIs, and database-backed verification.

Feel free to connect with me here: https://in.linkedin.com/in/amol-sadare
