# draakusa.github.io

[![pages-build-deployment](https://github.com/DraakUSA/draakusa.github.io/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/DraakUSA/draakusa.github.io/actions/workflows/pages/pages-build-deployment)

---

## 📌 About This Repository

This repository contains the source code for my personal website and professional portfolio, hosted via **GitHub Pages**. Built using **Jekyll** with the **Minimal Mistakes** theme, this site is a central hub for my diverse development work, ranging from software applications to hardware integration.

### Core Focus Areas:
* **Software Development:** A showcase of various programming projects, web tools, and general software engineering.
* **Firmware & Embedded Systems:** Custom C/C++ logic for microcontrollers like the ATtiny85.
* **Electronics & Automotive DIY:** Hardware hacking and DIY electronics, such as vehicle battery monitors and power management solutions.

---

## 🛠️ Running the Project

You can run this project locally using a Ruby environment or with Docker.

### 1. Local Development (Ruby)

Use this method if you have a local Ruby environment configured.

**Prerequisites:**
*   Ruby and Bundler installed.

**Commands:**

1.  **Install dependencies:**
    ```bash
    bundle install
    ```

2.  **Run the Jekyll server:**
    ```bash
    bundle exec jekyll serve
    ```
    The site will be available at `http://localhost:4000`.

### 2. Docker Development

Use this method for a containerized setup without installing Ruby locally.

**Prerequisites:**
*   Docker and Docker Compose installed.

**Commands:**

1.  **Build and run the container:**
    ```bash
    docker-compose up
    ```
    The site will be available at `http://localhost:4000`. The service includes live reloading.

2.  **Updating after Gemfile changes:**
    If you modify the `Gemfile`, you need to rebuild the image to install the new dependencies.
    ```bash
    docker-compose up --build
    ```

3.  **Stopping the container:**
    To stop and remove the running containers, press `Ctrl + C` or run:
    ```bash
    docker-compose down
    ```

## 💡 Useful Flags

You can append these flags to the `serve` command (e.g., `bundle exec jekyll serve --drafts --livereload`).

*   `--drafts`: Includes posts located in the `_drafts` folder.
*   `--unpublished`: Includes projects/posts where `published: false` is set.
*   `--future`: Publishes posts even if their date is in the future.
*   `--livereload`: Automatically refresh the browser on file changes.
*   `--force_polling`: Force file system polling, which can be necessary in some environments where automatic change detection fails.
