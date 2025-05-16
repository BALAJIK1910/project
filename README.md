# Project Responsive Web Design using Bootstrap
# Date:16-05-2025
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Famous Tech People</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            background: linear-gradient(135deg, #e3f0ff 0%, #fafcff 100%);
            min-height: 100vh;
        }

        .navbar-brand {
            font-weight: bold;
            letter-spacing: 1px;
            font-size: 1.7rem;
        }

        header {
            background: linear-gradient(90deg, #e3f0ff 0%, #b6e0fe 100%);
            border-bottom: 2px solid #0d6efd;
            box-shadow: 0 2px 8px rgba(13, 110, 253, 0.07);
        }

        .display-4 {
            font-weight: 700;
            color: #0d6efd;
            letter-spacing: 2px;
        }

        .card {
            box-shadow: 0 2px 12px rgba(0, 0, 0, 0.08);
            border-radius: 1.2rem;
            border: none;
            transition: transform 0.2s, box-shadow 0.2s;
            background: #fff;
        }

        .card:hover {
            transform: translateY(-8px) scale(1.04);
            box-shadow: 0 8px 32px rgba(13, 110, 253, 0.18);
        }

        .card-title {
            font-weight: 700;
            color: #0d6efd;
            font-size: 1.1rem;
        }

        .card-text {
            color: #555;
            font-size: 0.93rem;
        }

        .ratio img {
            border-radius: 50%;
            border: 3px solid #b6e0fe;
            box-shadow: 0 2px 8px rgba(13, 110, 253, 0.08);
        }

        .card-body {
            background: linear-gradient(90deg, #f8fbff 0%, #e3f0ff 100%);
            border-radius: 0 0 1.2rem 1.2rem;
        }

        footer {
            letter-spacing: 1px;
            font-size: 1rem;
        }

        @media (max-width: 576px) {
            .display-4 {
                font-size: 2rem;
            }

            .card {
                max-width: 100% !important;
            }
        }
    </style>
</head>

<body>
    <nav class="navbar navbar-expand-lg navbar-dark bg-primary shadow-sm">
        <div class="container-fluid">
            <a class="navbar-brand" href="#">MySite</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link active" href="#">Home</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <header class="py-5 text-center">
        <div class="container">
            <h1 class="display-4 mb-3">Famous Tech People</h1>
            <p class="lead text-secondary mb-0">Visionaries who shaped the world of technology</p>
        </div>
    </header>

    <section class="container my-5">
        <div class="row row-cols-2 row-cols-md-5 g-4 justify-content-center">
            <div class="col">
                <div class="card h-100 text-center" style="max-width: 160px; margin:auto;">
                    <div class="ratio ratio-1x1" style="height: 110px;">
                        <img src="steve.jpg" class="card-img-top object-fit-cover" alt="Steve Jobs"
                            style="object-fit: cover; width: 100%; height: 100%;">
                    </div>
                    <div class="card-body p-3">
                        <h6 class="card-title mb-1">Steve Jobs</h6>
                        <p class="card-text small">Co-founder of Apple Inc. and a pioneer of the personal computer
                            revolution.</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card h-100 text-center" style="max-width: 160px; margin:auto;">
                    <div class="ratio ratio-1x1" style="height: 110px;">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/a/a0/Bill_Gates_2018.jpg"
                            class="card-img-top object-fit-cover" alt="Bill Gates"
                            style="object-fit: cover; width: 100%; height: 100%;">
                    </div>
                    <div class="card-body p-3">
                        <h6 class="card-title mb-1">Bill Gates</h6>
                        <p class="card-text small">Co-founder of Microsoft and a leading philanthropist in technology
                            and health.</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card h-100 text-center" style="max-width: 160px; margin:auto;">
                    <div class="ratio ratio-1x1" style="height: 110px;">
                        <img src="Mark.jpg" class="card-img-top object-fit-cover" alt="Mark Zuckerberg"
                            style="object-fit: cover; width: 100%; height: 100%;">
                    </div>
                    <div class="card-body p-3">
                        <h6 class="card-title mb-1">Mark Zuckerberg</h6>
                        <p class="card-text small">Co-founder and CEO of Facebook, a major figure in social media
                            innovation.</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card h-100 text-center" style="max-width: 160px; margin:auto;">
                    <div class="ratio ratio-1x1" style="height: 110px;">
                        <img src="Susan.jpg" class="card-img-top object-fit-cover" alt="Susan Wojcicki"
                            style="object-fit: cover; width: 100%; height: 100%;">
                    </div>
                    <div class="card-body p-3">
                        <h6 class="card-title mb-1">Susan Wojcicki</h6>
                        <p class="card-text small">Former CEO of YouTube, influential in the growth of online video
                            platforms.</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card h-100 text-center" style="max-width: 160px; margin:auto;">
                    <div class="ratio ratio-1x1" style="height: 110px;">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/4/49/Elon_Musk_2015.jpg"
                            class="card-img-top object-fit-cover" alt="Elon Musk"
                            style="object-fit: cover; width: 100%; height: 100%;">
                    </div>
                    <div class="card-body p-3">
                        <h6 class="card-title mb-1">Elon Musk</h6>
                        <p class="card-text small">CEO of Tesla and SpaceX, known for innovations in electric cars and
                            space travel.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <footer class="bg-primary text-white text-center py-3 fixed-bottom shadow">
        &copy; 2025 Responsive Web Design Example
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</body>

</html>
```
# OUTPUT:

![alt text](<Screenshot 2025-05-16 223251.png>)

# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
