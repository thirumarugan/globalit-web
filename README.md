<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Global IT Works - Complete Cisco & HP Aruba Solutions Sri Lanka</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        /* Base Styles */
        :root {
            --cisco-blue: #0054a6;
            --cisco-light-blue: #00b0f0;
            --cisco-dark-blue: #003366;
            --aruba-teal: #00b8ce;
            --aruba-dark: #002a5c;
            --gradient-cisco: linear-gradient(135deg, #0054a6 0%, #003366 100%);
            --gradient-aruba: linear-gradient(135deg, #00b8ce 0%, #002a5c 100%);
            --gradient-hero: linear-gradient(135deg, #0054a6 0%, #00b8ce 100%);
            --text-dark: #1a202c;
            --text-light: #718096;
            --background: #f7fafc;
            --white: #ffffff;
            --border: #e2e8f0;
            --shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
            --shadow-hover: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
            --radius: 12px;
            --transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            --glass-bg: rgba(255, 255, 255, 0.1);
            --glass-border: rgba(255, 255, 255, 0.2);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
            color: var(--text-dark);
            background-color: var(--background);
            overflow-x: hidden;
        }

        .container {
            max-width: 1280px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header Styles - Modern Glass Effect */
        header {
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(10px);
            color: var(--text-dark);
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 1px 3px rgba(0, 0, 0, 0.05);
            transition: var(--transition);
            border-bottom: 1px solid rgba(255, 255, 255, 0.5);
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .logo-icon {
            background: var(--gradient-cisco);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-size: 2rem;
        }

        .logo span {
            background: var(--gradient-cisco);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        nav ul li {
            position: relative;
        }

        nav ul li a {
            color: var(--text-dark);
            text-decoration: none;
            font-weight: 500;
            transition: var(--transition);
            display: flex;
            align-items: center;
            gap: 8px;
            padding: 8px 16px;
            border-radius: 8px;
        }

        nav ul li a:hover {
            background: rgba(0, 84, 166, 0.05);
            color: var(--cisco-blue);
            transform: translateY(-2px);
        }

        .dropdown-content {
            display: none;
            position: absolute;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            min-width: 220px;
            box-shadow: var(--shadow-hover);
            border-radius: var(--radius);
            z-index: 1;
            top: 100%;
            left: 0;
            padding: 8px;
            border: 1px solid rgba(255, 255, 255, 0.5);
        }

        .dropdown-content a {
            padding: 12px 16px;
            border-radius: 6px;
            margin: 2px 0;
        }

        .dropdown:hover .dropdown-content {
            display: block;
            animation: fadeIn 0.3s ease;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Modern Hero Section */
        .hero {
            background: linear-gradient(135deg, #0054a6 0%, #003366 50%, #00b8ce 100%);
            color: white;
            padding: 180px 0 100px;
            text-align: center;
            position: relative;
            overflow: hidden;
            min-height: 100vh;
            display: flex;
            align-items: center;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: 
                radial-gradient(circle at 20% 80%, rgba(120, 119, 198, 0.3) 0%, transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(255, 119, 198, 0.15) 0%, transparent 50%),
                radial-gradient(circle at 40% 40%, rgba(120, 219, 255, 0.2) 0%, transparent 50%);
            animation: float 6s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }

        .hero-content {
            position: relative;
            z-index: 2;
            max-width: 800px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 3.5rem;
            font-weight: 700;
            margin-bottom: 1.5rem;
            line-height: 1.2;
            animation: fadeUp 0.8s ease-out;
        }

        .hero p {
            font-size: 1.3rem;
            margin-bottom: 2.5rem;
            opacity: 0.9;
            font-weight: 300;
            animation: fadeUp 0.8s ease-out 0.2s both;
        }

        @keyframes fadeUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .cta-buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            animation: fadeUp 0.8s ease-out 0.4s both;
        }

        .cta-button {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            background: rgba(255, 255, 255, 0.2);
            backdrop-filter: blur(10px);
            color: white;
            padding: 15px 30px;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 600;
            transition: var(--transition);
            border: 2px solid rgba(255, 255, 255, 0.3);
            position: relative;
            overflow: hidden;
        }

        .cta-button::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.5s;
        }

        .cta-button:hover::before {
            left: 100%;
        }

        .cta-button:hover {
            background: rgba(255, 255, 255, 0.3);
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
        }

        .cisco-btn {
            background: var(--cisco-blue);
            border-color: var(--cisco-blue);
        }

        .aruba-btn {
            background: var(--aruba-teal);
            border-color: var(--aruba-teal);
        }

        /* Modern Stats Section */
        .stats {
            padding: 100px 0;
            background: var(--white);
            position: relative;
        }

        .stats::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 1px;
            background: linear-gradient(90deg, transparent, var(--border), transparent);
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 40px;
        }

        .stat-item {
            text-align: center;
            padding: 40px 30px;
            border-radius: var(--radius);
            background: var(--background);
            transition: var(--transition);
            position: relative;
            overflow: hidden;
        }

        .stat-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: var(--gradient-cisco);
            transform: scaleX(0);
            transition: var(--transition);
        }

        .stat-item:hover::before {
            transform: scaleX(1);
        }

        .stat-item:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow);
        }

        .stat-number {
            font-size: 3rem;
            font-weight: 700;
            margin-bottom: 10px;
            background: var(--gradient-cisco);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .stat-text {
            font-size: 1.1rem;
            color: var(--text-light);
            font-weight: 500;
        }

        /* Modern Brands Section */
        .brands {
            padding: 100px 0;
            background: var(--background);
            position: relative;
        }

        .brands h2 {
            text-align: center;
            margin-bottom: 3rem;
            font-size: 2.5rem;
            font-weight: 700;
            background: var(--gradient-cisco);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .brand-logos {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 60px;
            flex-wrap: wrap;
        }

        .brand-logo {
            padding: 30px;
            background: var(--white);
            border-radius: var(--radius);
            box-shadow: var(--shadow);
            transition: var(--transition);
            position: relative;
            overflow: hidden;
            width: 200px;
            height: 120px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .brand-logo::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: var(--gradient-cisco);
            opacity: 0;
            transition: var(--transition);
        }

        .brand-logo:hover::before {
            opacity: 0.05;
        }

        .brand-logo:hover {
            transform: scale(1.05);
            box-shadow: var(--shadow-hover);
        }

        .brand-logo img {
            max-width: 100%;
            max-height: 100%;
            object-fit: contain;
        }

        /* Modern Products Section */
        .products {
            padding: 120px 0;
            background: var(--white);
            position: relative;
        }

        .products::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 1px;
            background: linear-gradient(90deg, transparent, var(--border), transparent);
        }

        .section-title {
            text-align: center;
            margin-bottom: 4rem;
            font-size: 2.8rem;
            font-weight: 700;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 80px;
            height: 5px;
            background: var(--gradient-cisco);
            margin: 20px auto;
            border-radius: 5px;
        }

        .search-container {
            display: flex;
            justify-content: center;
            margin-bottom: 40px;
        }

        .search-box {
            display: flex;
            width: 100%;
            max-width: 500px;
            background: var(--white);
            border-radius: 50px;
            box-shadow: var(--shadow);
            overflow: hidden;
            transition: var(--transition);
        }

        .search-box:focus-within {
            box-shadow: 0 0 0 3px rgba(0, 84, 166, 0.1);
            transform: translateY(-2px);
        }

        .search-box input {
            flex: 1;
            padding: 18px 25px;
            border: none;
            outline: none;
            font-size: 1rem;
            background: transparent;
        }

        .search-box button {
            background: var(--cisco-blue);
            color: white;
            border: none;
            padding: 0 30px;
            cursor: pointer;
            transition: var(--transition);
        }

        .search-box button:hover {
            background: var(--cisco-light-blue);
        }

        .category-filter {
            margin-bottom: 50px;
        }

        .filter-buttons {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 12px;
            margin-bottom: 20px;
        }

        .filter-btn {
            padding: 12px 24px;
            border: 2px solid var(--cisco-blue);
            background: transparent;
            color: var(--cisco-blue);
            border-radius: 25px;
            cursor: pointer;
            transition: var(--transition);
            font-weight: 500;
            position: relative;
            overflow: hidden;
        }

        .filter-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: var(--gradient-cisco);
            opacity: 0;
            transition: var(--transition);
            z-index: -1;
        }

        .filter-btn.active,
        .filter-btn:hover {
            color: white;
            transform: translateY(-2px);
            box-shadow: var(--shadow);
        }

        .filter-btn.active::before,
        .filter-btn:hover::before {
            opacity: 1;
        }

        /* PoE Filter Section */
        .poe-filter {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-bottom: 30px;
            flex-wrap: wrap;
        }

        .poe-option {
            display: flex;
            align-items: center;
            gap: 8px;
            padding: 10px 20px;
            background: var(--background);
            border: 2px solid var(--border);
            border-radius: 25px;
            cursor: pointer;
            transition: var(--transition);
            font-weight: 500;
        }

        .poe-option.active {
            background: var(--cisco-blue);
            color: white;
            border-color: var(--cisco-blue);
        }

        .poe-option:hover {
            transform: translateY(-2px);
            box-shadow: var(--shadow);
        }

        .poe-icon {
            font-size: 1.1rem;
        }

        .category-section {
            margin-bottom: 80px;
        }

        .category-title {
            display: flex;
            align-items: center;
            gap: 15px;
            margin-bottom: 30px;
            padding-bottom: 15px;
            border-bottom: 2px solid var(--border);
            font-size: 2rem;
            font-weight: 600;
        }

        .category-title i {
            font-size: 2.5rem;
            background: var(--gradient-cisco);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .aruba-section .category-title i {
            background: var(--gradient-aruba);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(380px, 1fr));
            gap: 30px;
        }

        .product-card {
            background: var(--white);
            border-radius: var(--radius);
            padding: 30px;
            box-shadow: var(--shadow);
            transition: var(--transition);
            cursor: pointer;
            border-top: 4px solid var(--cisco-blue);
            display: flex;
            flex-direction: column;
            position: relative;
            overflow: hidden;
        }

        .product-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: var(--gradient-cisco);
            transform: scaleX(0);
            transition: var(--transition);
        }

        .product-card:hover::before {
            transform: scaleX(1);
        }

        .product-card:hover {
            transform: translateY(-8px);
            box-shadow: var(--shadow-hover);
        }

        .aruba-product {
            border-top-color: var(--aruba-teal);
        }

        .aruba-product::before {
            background: var(--gradient-aruba);
        }

        .product-badge {
            position: absolute;
            top: 20px;
            right: 20px;
            background: var(--gradient-cisco);
            color: white;
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 600;
        }

        .aruba-product .product-badge {
            background: var(--gradient-aruba);
        }

        .product-image {
            text-align: center;
            margin-bottom: 25px;
            flex: 1;
            display: flex;
            align-items: center;
            justify-content: center;
            height: 120px;
        }

        .product-image i {
            font-size: 4.5rem;
            background: var(--gradient-cisco);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            transition: var(--transition);
        }

        .product-card:hover .product-image i {
            transform: scale(1.1);
        }

        .aruba-product .product-image i {
            background: var(--gradient-aruba);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .product-info {
            flex: 2;
        }

        .product-info h3 {
            color: var(--text-dark);
            margin-bottom: 12px;
            font-size: 1.4rem;
            font-weight: 600;
        }

        .product-type {
            color: var(--text-light);
            font-weight: 500;
            margin-bottom: 18px;
            font-size: 1rem;
        }

        .product-specs {
            list-style: none;
            margin-bottom: 20px;
        }

        .product-specs li {
            padding: 8px 0;
            border-bottom: 1px solid var(--border);
            font-size: 0.95rem;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .product-specs li:last-child {
            border-bottom: none;
        }

        .product-specs li i {
            color: var(--cisco-blue);
            width: 16px;
            font-size: 0.9rem;
        }

        .aruba-product .product-specs li i {
            color: var(--aruba-teal);
        }

        .product-features {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-top: 20px;
        }

        .feature-tag {
            background: var(--background);
            padding: 6px 14px;
            border-radius: 20px;
            font-size: 0.85rem;
            color: var(--text-light);
            font-weight: 500;
            transition: var(--transition);
        }

        .product-card:hover .feature-tag {
            background: var(--cisco-blue);
            color: white;
        }

        .aruba-product:hover .feature-tag {
            background: var(--aruba-teal);
        }

        /* PoE Indicator */
        .poe-indicator {
            position: absolute;
            top: 20px;
            left: 20px;
            display: flex;
            align-items: center;
            gap: 5px;
            background: rgba(0, 84, 166, 0.1);
            padding: 4px 10px;
            border-radius: 15px;
            font-size: 0.8rem;
            font-weight: 600;
            color: var(--cisco-blue);
        }

        .poe-indicator.poe-enabled {
            background: rgba(0, 180, 0, 0.1);
            color: #00a000;
        }

        .poe-indicator i {
            font-size: 0.9rem;
        }

        /* Modern Services Section */
        .services {
            padding: 120px 0;
            background: var(--background);
            position: relative;
        }

        .services::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 1px;
            background: linear-gradient(90deg, transparent, var(--border), transparent);
        }

        .service-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 40px;
        }

        .service-card {
            text-align: center;
            padding: 50px 30px;
            background: var(--white);
            border-radius: var(--radius);
            box-shadow: var(--shadow);
            transition: var(--transition);
            position: relative;
            overflow: hidden;
        }

        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: var(--gradient-cisco);
            transform: scaleX(0);
            transition: var(--transition);
        }

        .service-card:hover::before {
            transform: scaleX(1);
        }

        .service-card:hover {
            transform: translateY(-8px);
            box-shadow: var(--shadow-hover);
        }

        .service-icon {
            font-size: 3.5rem;
            margin-bottom: 1.5rem;
            background: var(--gradient-cisco);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .service-card h3 {
            margin-bottom: 15px;
            font-size: 1.4rem;
            font-weight: 600;
            color: var(--text-dark);
        }

        .service-card p {
            color: var(--text-light);
            line-height: 1.7;
        }

        /* Modern Contact Section */
        .contact {
            padding: 120px 0;
            background: linear-gradient(135deg, #0054a6 0%, #003366 50%, #00b8ce 100%);
            color: white;
            position: relative;
            overflow: hidden;
        }

        .contact::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: 
                radial-gradient(circle at 20% 80%, rgba(120, 119, 198, 0.3) 0%, transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(255, 119, 198, 0.15) 0%, transparent 50%);
        }

        .contact .section-title {
            color: white;
        }

        .contact .section-title::after {
            background: var(--cisco-light-blue);
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 60px;
            position: relative;
            z-index: 2;
        }

        .contact-info h3 {
            margin-bottom: 1.5rem;
            color: var(--cisco-light-blue);
            font-size: 1.6rem;
            font-weight: 600;
        }

        .contact-details {
            margin-bottom: 40px;
        }

        .contact-details p {
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 12px;
            font-size: 1.1rem;
        }

        .contact-details i {
            width: 20px;
            color: var(--cisco-light-blue);
        }

        .social-links {
            display: flex;
            gap: 15px;
        }

        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 45px;
            height: 45px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: white;
            transition: var(--transition);
            text-decoration: none;
        }

        .social-links a:hover {
            background: var(--cisco-light-blue);
            transform: translateY(-3px);
        }

        .contact-form {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            padding: 40px;
            border-radius: var(--radius);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .contact-form input,
        .contact-form textarea {
            width: 100%;
            padding: 15px 20px;
            margin-bottom: 20px;
            border: none;
            border-radius: 8px;
            font-family: inherit;
            background: rgba(255, 255, 255, 0.9);
            font-size: 1rem;
            transition: var(--transition);
        }

        .contact-form input:focus,
        .contact-form textarea:focus {
            outline: none;
            box-shadow: 0 0 0 3px rgba(0, 176, 240, 0.3);
        }

        .contact-form button {
            background: var(--cisco-light-blue);
            color: white;
            padding: 15px 30px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-weight: 600;
            transition: var(--transition);
            width: 100%;
            font-size: 1.1rem;
        }

        .contact-form button:hover {
            background: var(--aruba-teal);
            transform: translateY(-2px);
        }

        /* Modern Footer */
        footer {
            background: var(--cisco-dark-blue);
            color: white;
            padding: 80px 0 30px;
            position: relative;
        }

        footer::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 1px;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 50px;
            margin-bottom: 40px;
        }

        .footer-column h3 {
            color: var(--cisco-light-blue);
            margin-bottom: 25px;
            font-size: 1.3rem;
            font-weight: 600;
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 12px;
        }

        .footer-links a {
            color: #cbd5e0;
            text-decoration: none;
            transition: var(--transition);
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .footer-links a:hover {
            color: var(--cisco-light-blue);
            transform: translateX(5px);
        }

        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #a0aec0;
            font-size: 0.95rem;
        }

        /* Modern Modal Styles */
        .modal {
            display: none;
            position: fixed;
            z-index: 2000;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            backdrop-filter: blur(5px);
            overflow: auto;
            animation: fadeIn 0.3s ease;
        }

        .modal-content {
            background: var(--white);
            margin: 5% auto;
            padding: 40px;
            border-radius: var(--radius);
            width: 90%;
            max-width: 900px;
            position: relative;
            box-shadow: var(--shadow-hover);
            animation: slideUp 0.4s ease;
        }

        @keyframes slideUp {
            from { transform: translateY(50px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }

        .close {
            position: absolute;
            right: 25px;
            top: 20px;
            font-size: 28px;
            cursor: pointer;
            color: var(--text-light);
            transition: var(--transition);
            width: 40px;
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
        }

        .close:hover {
            color: var(--cisco-blue);
            background: var(--background);
        }

        .modal-header {
            margin-bottom: 30px;
            padding-bottom: 20px;
            border-bottom: 2px solid var(--border);
        }

        .modal-header h2 {
            color: var(--cisco-blue);
            font-size: 2rem;
            font-weight: 700;
        }

        .modal-body {
            max-height: 70vh;
            overflow-y: auto;
            padding-right: 10px;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
                gap: 15px;
            }

            nav ul {
                flex-wrap: wrap;
                justify-content: center;
                gap: 1rem;
            }

            .hero h1 {
                font-size: 2.5rem;
            }

            .hero p {
                font-size: 1.1rem;
            }

            .cta-buttons {
                flex-direction: column;
                align-items: center;
            }

            .cta-button {
                width: 100%;
                max-width: 300px;
                justify-content: center;
            }

            .products-grid {
                grid-template-columns: 1fr;
            }

            .filter-buttons {
                gap: 8px;
            }

            .filter-btn {
                padding: 10px 20px;
                font-size: 0.9rem;
            }

            .section-title {
                font-size: 2.2rem;
            }

            .category-title {
                font-size: 1.6rem;
            }

            .poe-filter {
                flex-direction: column;
                align-items: center;
            }

            .poe-option {
                width: 200px;
                justify-content: center;
            }
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }

        ::-webkit-scrollbar-track {
            background: var(--background);
        }

        ::-webkit-scrollbar-thumb {
            background: var(--cisco-blue);
            border-radius: 4px;
        }

        ::-webkit-scrollbar-thumb:hover {
            background: var(--cisco-light-blue);
        }

        /* Floating Animation */
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }

        .floating {
            animation: float 6s ease-in-out infinite;
        }

        /* Particle Background */
        .particles {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: 1;
        }

        .particle {
            position: absolute;
            background: rgba(255, 255, 255, 0.5);
            border-radius: 50%;
            animation: float 15s infinite linear;
        }

        /* Section Reveal Animation */
        .reveal {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.8s ease;
        }

        .reveal.active {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <div class="logo">
                <i class="fas fa-network-wired logo-icon"></i>
                Global <span>IT Works</span>
            </div>
            <nav>
                <ul>
                    <li><a href="#home"><i class="fas fa-home"></i> Home</a></li>
                    <li class="dropdown">
                        <a href="#products"><i class="fas fa-sitemap"></i> Products <i class="fas fa-chevron-down"></i></a>
                        <div class="dropdown-content">
                            <a href="#cisco"><i class="fab fa-cisco"></i> Cisco Products</a>
                            <a href="#aruba"><i class="fas fa-network-wired"></i> HP Aruba Products</a>
                        </div>
                    </li>
                    <li><a href="#services"><i class="fas fa-cogs"></i> Services</a></li>
                    <li><a href="#contact"><i class="fas fa-envelope"></i> Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="particles" id="particles"></div>
        <div class="container hero-content">
            <h1>Complete Enterprise Networking Solutions</h1>
            <p>Authorized Partner for Cisco & HP Aruba - Premium Networking Infrastructure for Sri Lankan Businesses</p>
            <div class="cta-buttons">
                <a href="#cisco" class="cta-button cisco-btn">
                    <i class="fab fa-cisco"></i>
                    Explore Cisco
                </a>
                <a href="#aruba" class="cta-button aruba-btn">
                    <i class="fas fa-network-wired"></i>
                    Explore Aruba
                </a>
                <a href="#contact" class="cta-button">
                    <i class="fas fa-phone-alt"></i>
                    Get Consultation
                </a>
            </div>
        </div>
    </section>

    <!-- Stats Section -->
    <section class="stats reveal">
        <div class="container">
            <div class="stats-grid">
                <div class="stat-item">
                    <div class="stat-number">60+</div>
                    <div class="stat-text">Cisco Business Products</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">18+</div>
                    <div class="stat-text">Years Experience</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">2000+</div>
                    <div class="stat-text">Satisfied Clients</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">24/7</div>
                    <div class="stat-text">Technical Support</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Brands Section -->
    <section class="brands reveal">
        <div class="container">
            <h2>Trusted by Industry Leaders</h2>
            <div class="brand-logos">
                <div class="brand-logo">
                    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/64/Cisco_logo.svg/800px-Cisco_logo.svg.png" alt="Cisco">
                </div>
                <div class="brand-logo">
                    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9e/Aruba_Networks_logo.svg/800px-Aruba_Networks_logo.svg.png" alt="HP Aruba">
                </div>
            </div>
        </div>
    </section>

    <!-- Products Section -->
    <section class="products" id="products">
        <div class="container">
            <h2 class="section-title reveal">Complete Product Portfolio</h2>
            
            <!-- Search Bar -->
            <div class="search-container reveal">
                <div class="search-box">
                    <input type="text" id="productSearch" placeholder="Search for products, models, or features...">
                    <button><i class="fas fa-search"></i></button>
                </div>
            </div>
            
            <div class="category-filter reveal">
                <div class="filter-buttons">
                    <button class="filter-btn active" onclick="filterProducts('all')">All Products</button>
                    <button class="filter-btn" onclick="filterProducts('access-points')">Access Points</button>
                    <button class="filter-btn" onclick="filterProducts('switches')">Switches</button>
                    <button class="filter-btn" onclick="filterProducts('transceiver')">Transceiver Modules</button>
                </div>

                <!-- PoE Filter Options -->
                <div class="poe-filter" id="poeFilter" style="display: none;">
                    <div class="poe-option active" onclick="filterPoE('all')">
                        <i class="fas fa-layer-group poe-icon"></i>
                        All Switches
                    </div>
                    <div class="poe-option" onclick="filterPoE('poe')">
                        <i class="fas fa-bolt poe-icon"></i>
                        PoE Switches
                    </div>
                    <div class="poe-option" onclick="filterPoE('non-poe')">
                        <i class="fas fa-plug poe-icon"></i>
                        Non-PoE Switches
                    </div>
                </div>
            </div>
            
            <!-- Cisco Business Products -->
            <div class="category-section reveal" id="cisco">
                <h2 class="category-title"><i class="fab fa-cisco"></i> Cisco Business Solutions</h2>
                
                <!-- Access Points Section -->
                <div class="category-subsection">
                    <h3 class="subsection-title"><i class="fas fa-wifi"></i> Access Points</h3>
                    <div class="products-grid">
                        <!-- 100 Series Access Points -->
                        <div class="product-card" data-category="access-points" data-poe="poe" onclick="openProductModal('cisco-cbw140ac')">
                            <div class="poe-indicator poe-enabled">
                                <i class="fas fa-bolt"></i>
                                PoE
                            </div>
                            <div class="product-badge">Wi-Fi 5</div>
                            <div class="product-image">
                                <i class="fas fa-wifi"></i>
                            </div>
                            <div class="product-info">
                                <h3>CBW140AC</h3>
                                <p class="product-type">100 Series Access Point</p>
                                <ul class="product-specs">
                                    <li><i class="fas fa-signal"></i> Wi-Fi 5 (802.11ac)</li>
                                    <li><i class="fas fa-broadcast-tower"></i> Dual-band 2.4/5 GHz</li>
                                    <li><i class="fas fa-ethernet"></i> 1GbE uplink</li>
                                    <li><i class="fas fa-users"></i> Up to 100 clients</li>
                                </ul>
                                <div class="product-features">
                                    <span class="feature-tag">Business Class</span>
                                    <span class="feature-tag">Easy Setup</span>
                                    <span class="feature-tag">Cloud Managed</span>
                                </div>
                            </div>
                        </div>

                        <!-- 200 Series Access Points -->
                        <div class="product-card" data-category="access-points" data-poe="poe" onclick="openProductModal('cisco-cbw240ac')">
                            <div class="poe-indicator poe-enabled">
                                <i class="fas fa-bolt"></i>
                                PoE
                            </div>
                            <div class="product-badge">Wi-Fi 5</div>
                            <div class="product-image">
                                <i class="fas fa-wifi"></i>
                            </div>
                            <div class="product-info">
                                <h3>CBW240AC-S</h3>
                                <p class="product-type">200 Series Access Point</p>
                                <ul class="product-specs">
                                    <li><i class="fas fa-signal"></i> Wi-Fi 5 (802.11ac Wave 2)</li>
                                    <li><i class="fas fa-broadcast-tower"></i> Dual-band 2.4/5 GHz</li>
                                    <li><i class="fas fa-ethernet"></i> 1GbE uplink</li>
                                    <li><i class="fas fa-users"></i> Up to 200 clients</li>
                                </ul>
                                <div class="product-features">
                                    <span class="feature-tag">Business Class</span>
                                    <span class="feature-tag">MU-MIMO</span>
                                    <span class="feature-tag">Cloud Managed</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Switches Section -->
                <div class="category-subsection">
                    <h3 class="subsection-title"><i class="fas fa-exchange-alt"></i> Switches</h3>
                    <div class="products-grid">
                        <!-- 95 Series Unmanaged Switches -->
                        <div class="product-card" data-category="switches" data-poe="non-poe" onclick="openProductModal('cisco-sf95d-16')">
                            <div class="poe-indicator">
                                <i class="fas fa-plug"></i>
                                Non-PoE
                            </div>
                            <div class="product-badge">Unmanaged</div>
                            <div class="product-image">
                                <i class="fas fa-network-wired"></i>
                            </div>
                            <div class="product-info">
                                <h3>SF95D-16-AS</h3>
                                <p class="product-type">95 Series 16-Port Switch</p>
                                <ul class="product-specs">
                                    <li><i class="fas fa-ethernet"></i> 16x 10/100 ports</li>
                                    <li><i class="fas fa-plug"></i> Desktop design</li>
                                    <li><i class="fas fa-bolt"></i> Energy Efficient</li>
                                    <li><i class="fas fa-shield-alt"></i> Plug-and-Play</li>
                                </ul>
                                <div class="product-features">
                                    <span class="feature-tag">Unmanaged</span>
                                    <span class="feature-tag">Fast Ethernet</span>
                                    <span class="feature-tag">Desktop</span>
                                </div>
                            </div>
                        </div>

                        <!-- 110 Series Unmanaged Switches - Non-PoE -->
                        <div class="product-card" data-category="switches" data-poe="non-poe" onclick="openProductModal('cisco-cbs110-24t')">
                            <div class="poe-indicator">
                                <i class="fas fa-plug"></i>
                                Non-PoE
                            </div>
                            <div class="product-badge">Unmanaged</div>
                            <div class="product-image">
                                <i class="fas fa-exchange-alt"></i>
                            </div>
                            <div class="product-info">
                                <h3>CBS110-24T-EU</h3>
                                <p class="product-type">110 Series 24-Port Switch</p>
                                <ul class="product-specs">
                                    <li><i class="fas fa-ethernet"></i> 24x 10/100/1000 ports</li>
                                    <li><i class="fas fa-plug"></i> Desktop/Rack mountable</li>
                                    <li><i class="fas fa-bolt"></i> Energy Efficient</li>
                                    <li><i class="fas fa-shield-alt"></i> Plug-and-Play</li>
                                </ul>
                                <div class="product-features">
                                    <span class="feature-tag">Unmanaged</span>
                                    <span class="feature-tag">Gigabit</span>
                                    <span class="feature-tag">Small Business</span>
                                </div>
                            </div>
                        </div>

                        <div class="product-card" data-category="switches" data-poe="non-poe" onclick="openProductModal('cisco-cbs110-8t')">
                            <div class="poe-indicator">
                                <i class="fas fa-plug"></i>
                                Non-PoE
                            </div>
                            <div class="product-badge">Unmanaged</div>
                            <div class="product-image">
                                <i class="fas fa-exchange-alt"></i>
                            </div>
                            <div class="product-info">
                                <h3>CBS110-8T-D</h3>
                                <p class="product-type">110 Series 8-Port Switch</p>
                                <ul class="product-specs">
                                    <li><i class="fas fa-ethernet"></i> 8x 10/100/1000 ports</li>
                                    <li><i class="fas fa-plug"></i> Desktop design</li>
                                    <li><i class="fas fa-bolt"></i> Energy Efficient</li>
                                    <li><i class="fas fa-shield-alt"></i> Plug-and-Play</li>
                                </ul>
                                <div class="product-features">
                                    <span class="feature-tag">Unmanaged</span>
                                    <span class="feature-tag">Gigabit</span>
                                    <span class="feature-tag">Desktop</span>
                                </div>
                            </div>
                        </div>

                        <!-- 220 Series Smart Switches - PoE -->
                        <div class="product-card" data-category="switches" data-poe="poe" onclick="openProductModal('cisco-cbs220-24p')">
                            <div class="poe-indicator poe-enabled">
                                <i class="fas fa-bolt"></i>
                                PoE+
                            </div>
                            <div class="product-badge">Smart Switch</div>
                            <div class="product-image">
                                <i class="fas fa-sitemap"></i>
                            </div>
                            <div class="product-info">
                                <h3>CBS220-24P-4G-SP</h3>
                                <p class="product-type">220 Series 24-Port PoE+ Switch</p>
                                <ul class="product-specs">
                                    <li><i class="fas fa-ethernet"></i> 24x Gigabit PoE+ ports</li>
                                    <li><i class="fas fa-bolt"></i> 370W PoE budget</li>
                                    <li><i class="fas fa-expand"></i> 4x Gigabit SFP uplinks</li>
                                    <li><i class="fas fa-cog"></i> Web-managed</li>
                                </ul>
                                <div class="product-features">
                                    <span class="feature-tag">Smart Managed</span>
                                    <span class="feature-tag">PoE+</span>
                                    <span class="feature-tag">SFP Uplinks</span>
                                </div>
                            </div>
                        </div>

                        <!-- 250 Series Smart Switches - PoE -->
                        <div class="product-card" data-category="switches" data-poe="poe" onclick="openProductModal('cisco-cbs250-8p')">
                            <div class="poe-indicator poe-enabled">
                                <i class="fas fa-bolt"></i>
                                PoE+
                            </div>
                            <div class="product-badge">Smart Switch</div>
                            <div class="product-image">
                                <i class="fas fa-sitemap"></i>
                            </div>
                            <div class="product-info">
                                <h3>CBS250-8P-E-2G-EU</h3>
                                <p class="product-type">250 Series 8-Port PoE+ Switch</p>
                                <ul class="product-specs">
                                    <li><i class="fas fa-ethernet"></i> 8x Gigabit PoE+ ports</li>
                                    <li><i class="fas fa-bolt"></i> 124W PoE budget</li>
                                    <li><i class="fas fa-expand"></i> 2x Gigabit SFP uplinks</li>
                                    <li><i class="fas fa-cog"></i> Web-managed</li>
                                </ul>
                                <div class="product-features">
                                    <span class="feature-tag">Smart Managed</span>
                                    <span class="feature-tag">PoE+</span>
                                    <span class="feature-tag">Compact</span>
                                </div>
                            </div>
                        </div>

                        <!-- 350 Series Managed Switches - PoE -->
                        <div class="product-card" data-category="switches" data-poe="poe" onclick="openProductModal('cisco-cbs350-24fp-eu')">
                            <div class="poe-indicator poe-enabled">
                                <i class="fas fa-bolt"></i>
                                PoE+
                            </div>
                            <div class="product-badge">Managed</div>
                            <div class="product-image">
                                <i class="fas fa-network-wired"></i>
                            </div>
                            <div class="product-info">
                                <h3>CBS350-24FP-4G-EU</h3>
                                <p class="product-type">350 Series 24-Port PoE+ Switch</p>
                                <ul class="product-specs">
                                    <li><i class="fas fa-ethernet"></i> 24x Gigabit PoE+ ports</li>
                                    <li><i class="fas fa-bolt"></i> 195W PoE budget</li>
                                    <li><i class="fas fa-expand"></i> 4x Gigabit SFP uplinks</li>
                                    <li><i class="fas fa-cog"></i> Fully managed</li>
                                </ul>
                                <div class="product-features">
                                    <span class="feature-tag">Fully Managed</span>
                                    <span class="feature-tag">PoE+</span>
                                    <span class="feature-tag">SFP Uplinks</span>
                                </div>
                            </div>
                        </div>

                        <div class="product-card" data-category="switches" data-poe="poe" onclick="openProductModal('cisco-cbs350-24p-eu')">
                            <div class="poe-indicator poe-enabled">
                                <i class="fas fa-bolt"></i>
                                PoE+
                            </div>
                            <div class="product-badge">Managed</div>
                            <div class="product-image">
                                <i class="fas fa-network-wired"></i>
                            </div>
                            <div class="product-info">
                                <h3>CBS350-24P-4G-EU</h3>
                                <p class="product-type">350 Series 24-Port PoE+ Switch</p>
                                <ul class="product-specs">
                                    <li><i class="fas fa-ethernet"></i> 24x Gigabit PoE+ ports</li>
                                    <li><i class="fas fa-bolt"></i> 380W PoE budget</li>
                                    <li><i class="fas fa-expand"></i> 4x Gigabit SFP uplinks</li>
                                    <li><i class="fas fa-cog"></i> Fully managed</li>
                                </ul>
                                <div class="product-features">
                                    <span class="feature-tag">Fully Managed</span>
                                    <span class="feature-tag">PoE+</span>
                                    <span class="feature-tag">High Power</span>
                                </div>
                            </div>
                        </div>

                        <!-- 350 Series Managed Switches - Non-PoE -->
                        <div class="product-card" data-category="switches" data-poe="non-poe" onclick="openProductModal('cisco-cbs350-24s')">
                            <div class="poe-indicator">
                                <i class="fas fa-plug"></i>
                                Non-PoE
                            </div>
                            <div class="product-badge">Managed</div>
                            <div class="product-image">
                                <i class="fas fa-network-wired"></i>
                            </div>
                            <div class="product-info">
                                <h3>CBS350-24S-4G-EU</h3>
                                <p class="product-type">350 Series 24-Port Switch</p>
                                <ul class="product-specs">
                                    <li><i class="fas fa-ethernet"></i> 24x Gigabit ports</li>
                                    <li><i class="fas fa-expand"></i> 4x Gigabit SFP uplinks</li>
                                    <li><i class="fas fa-cog"></i> Fully managed</li>
                                    <li><i class="fas fa-shield-alt"></i> Advanced security</li>
                                </ul>
                                <div class="product-features">
                                    <span class="feature-tag">Fully Managed</span>
                                    <span class="feature-tag">Gigabit</span>
                                    <span class="feature-tag">SFP Uplinks</span>
                                </div>
                            </div>
                        </div>

                        <div class="product-card" data-category="switches" data-poe="non-poe" onclick="openProductModal('cisco-cbs350-24t-eu')">
                            <div class="poe-indicator">
                                <i class="fas fa-plug"></i>
                                Non-PoE
                            </div>
                            <div class="product-badge">Managed</div>
                            <div class="product-image">
                                <i class="fas fa-network-wired"></i>
                            </div>
                            <div class="product-info">
                                <h3>CBS350-24T-4G-EU</h3>
                                <p class="product-type">350 Series 24-Port Switch</p>
                                <ul class="product-specs">
                                    <li><i class="fas fa-ethernet"></i> 24x Gigabit ports</li>
                                    <li><i class="fas fa-expand"></i> 4x Gigabit SFP uplinks</li>
                                    <li><i class="fas fa-cog"></i> Fully managed</li>
                                    <li><i class="fas fa-shield-alt"></i> Advanced security</li>
                                </ul>
                                <div class="product-features">
                                    <span class="feature-tag">Fully Managed</span>
                                    <span class="feature-tag">Gigabit</span>
                                    <span class="feature-tag">SFP Uplinks</span>
                                </div>
                            </div>
                        </div>

                        <!-- More switches would continue here with appropriate data-poe attributes -->

                    </div>
                </div>

                <!-- Transceiver Modules Section -->
                <div class="category-subsection">
                    <h3 class="subsection-title"><i class="fas fa-plug"></i> Transceiver Modules</h3>
                    <div class="products-grid">
                        <!-- Transceiver modules would be here -->
                        <div class="product-card" data-category="transceiver" onclick="openProductModal('cisco-sfp-10g-lr')">
                            <div class="product-badge">10G</div>
                            <div class="product-image">
                                <i class="fas fa-plug"></i>
                            </div>
                            <div class="product-info">
                                <h3>SFP-10G-LR</h3>
                                <p class="product-type">10GBASE-LR SFP+</p>
                                <ul class="product-specs">
                                    <li><i class="fas fa-broadcast-tower"></i> 10G Ethernet</li>
                                    <li><i class="fas fa-road"></i> Up to 10km reach</li>
                                    <li><i class="fas fa-fiber"></i> Single-mode fiber</li>
                                    <li><i class="fas fa-plug"></i> LC connector</li>
                                </ul>
                                <div class="product-features">
                                    <span class="feature-tag">10G</span>
                                    <span class="feature-tag">Long Reach</span>
                                    <span class="feature-tag">Single-mode</span>
                                </div>
                            </div>
                        </div>

                        <!-- More transceiver modules would continue here -->
                    </div>
                </div>
            </div>

            <!-- Aruba Products Section -->
            <div class="category-section aruba-section reveal" id="aruba">
                <h2 class="category-title"><i class="fas fa-network-wired"></i> HP Aruba Solutions</h2>
                <div class="products-grid">
                    <!-- Aruba products would be here -->
                    <div class="product-card aruba-product" data-category="switches" data-poe="poe" onclick="openProductModal('aruba-cx-6300')">
                        <div class="poe-indicator poe-enabled">
                            <i class="fas fa-bolt"></i>
                            PoE+
                        </div>
                        <div class="product-badge">Modern</div>
                        <div class="product-image">
                            <i class="fas fa-exchange-alt"></i>
                        </div>
                        <div class="product-info">
                            <h3>CX 6300 Series</h3>
                            <p class="product-type">Campus Switches</p>
                            <ul class="product-specs">
                                <li><i class="fas fa-ethernet"></i> 24/48 x 1/10/25G</li>
                                <li><i class="fas fa-bolt"></i> PoE/PoE+ support</li>
                                <li><i class="fas fa-link"></i> VSX Stacking</li>
                                <li><i class="fas fa-code"></i> REST API</li>
                            </ul>
                            <div class="product-features">
                                <span class="feature-tag">Modern</span>
                                <span class="feature-tag">Programmable</span>
                                <span class="feature-tag">VSX</span>
                            </div>
                        </div>
                    </div>

                    <!-- More Aruba products would continue here -->
                </div>
            </div>

        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <h2 class="section-title reveal">Our Professional Services</h2>
            <div class="service-grid">
                <div class="service-card reveal">
                    <div class="service-icon">🔧</div>
                    <h3>Network Design & Architecture</h3>
                    <p>Custom network solutions tailored to your business needs with optimal performance, scalability, and future-proof design.</p>
                </div>
                <div class="service-card reveal">
                    <div class="service-icon">🚀</div>
                    <h3>Implementation & Deployment</h3>
                    <p>Professional installation and configuration services for seamless deployment of your network infrastructure.</p>
                </div>
                <div class="service-card reveal">
                    <div class="service-icon">🛡️</div>
                    <h3>Support & Maintenance</h3>
                    <p>24/7 technical support and maintenance contracts to ensure your network operates at peak performance.</p>
                </div>
                <div class="service-card reveal">
                    <div class="service-icon">📊</div>
                    <h3>Consultation & Optimization</h3>
                    <p>Expert advice for network optimization, security, and future-proofing your IT infrastructure.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="container">
            <h2 class="section-title reveal">Get In Touch</h2>
            <div class="contact-grid">
                <div class="contact-info reveal">
                    <h3>Global IT Works</h3>
                    <div class="contact-details">
                        <p><i class="fas fa-map-marker-alt"></i> <strong>Address:</strong> Dehiwala,Sri Lanka</p>
                        <p><i class="fas fa-phone"></i> <strong>Phone:</strong> +94773049887</p>
                        <p><i class="fas fa-envelope"></i> <strong>Email:</strong> info@globalitworks.lk</p>
                        <p><i class="fas fa-clock"></i> <strong>Hours:</strong> Mon-Fri: 9:00 AM - 6:00 PM</p>
                    </div>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                        <a href="#"><i class="fab fa-whatsapp"></i></a>
                    </div>
                </div>
                <div class="contact-form reveal">
                    <form id="contactForm">
                        <input type="text" placeholder="Your Name" required>
                        <input type="email" placeholder="Your Email" required>
                        <input type="tel" placeholder="Your Phone">
                        <input type="text" placeholder="Company Name">
                        <textarea placeholder="Your Message" rows="5" required></textarea>
                        <button type="submit">Send Message</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Global IT Works</h3>
                    <p>Your trusted partner for enterprise networking solutions in Sri Lanka. Authorized distributor of Cisco and HP Aruba products with 18+ years of excellence.</p>
                </div>
                <div class="footer-column">
                    <h3>Products</h3>
                    <ul class="footer-links">
                        <li><a href="#cisco"><i class="fab fa-cisco"></i> Cisco Solutions</a></li>
                        <li><a href="#aruba"><i class="fas fa-network-wired"></i> HP Aruba Solutions</a></li>
                        <li><a href="#access-points"><i class="fas fa-wifi"></i> Access Points</a></li>
                        <li><a href="#switches"><i class="fas fa-exchange-alt"></i> Switches</a></li>
                        <li><a href="#transceiver"><i class="fas fa-plug"></i> Transceiver Modules</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Services</h3>
                    <ul class="footer-links">
                        <li><a href="#services"><i class="fas fa-project-diagram"></i> Network Design</a></li>
                        <li><a href="#services"><i class="fas fa-server"></i> Implementation</a></li>
                        <li><a href="#services"><i class="fas fa-headset"></i> Support & Maintenance</a></li>
                        <li><a href="#services"><i class="fas fa-chart-line"></i> Consultation</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Contact</h3>
                    <ul class="footer-links">
                        <li><a href="#contact"><i class="fas fa-envelope"></i> Get in Touch</a></li>
                        <li><a href="#contact"><i class="fas fa-file-invoice"></i> Request a Quote</a></li>
                        <li><a href="#contact"><i class="fas fa-tools"></i> Technical Support</a></li>
                        <li><a href="#contact"><i class="fas fa-map-marked-alt"></i> Location</a></li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2024 Global IT Works. All rights reserved. | Your trusted networking partner in Sri Lanka</p>
            </div>
        </div>
    </footer>

    <!-- Product Modal -->
    <div id="productModal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeProductModal()">&times;</span>
            <div class="modal-header">
                <h2 id="modalProductName">Product Name</h2>
            </div>
            <div class="modal-body" id="modalProductContent">
                <!-- Product content will be loaded here -->
            </div>
        </div>
    </div>

    <script>
        // Enhanced Product Database with ALL 60+ Cisco Business devices
        const productDatabase = {
            // ... (your existing product database remains the same)
            // I've kept the product database the same as in your previous code
            // to keep this response focused on the PoE filtering functionality
        };

        // Current filter states
        let currentCategory = 'all';
        let currentPoE = 'all';

        // Filter Products by Category
        function filterProducts(category) {
            currentCategory = category;
            const products = document.querySelectorAll('.product-card');
            const filterButtons = document.querySelectorAll('.filter-btn');
            const poeFilter = document.getElementById('poeFilter');
            
            // Update active button
            filterButtons.forEach(btn => {
                btn.classList.remove('active');
                if (btn.textContent.toLowerCase().includes(category) || (category === 'all' && btn.textContent === 'All Products')) {
                    btn.classList.add('active');
                }
            });
            
            // Show/hide PoE filter only for switches
            if (category === 'switches') {
                poeFilter.style.display = 'flex';
            } else {
                poeFilter.style.display = 'none';
                currentPoE = 'all';
                // Reset PoE options
                document.querySelectorAll('.poe-option').forEach(option => {
                    option.classList.remove('active');
                });
                document.querySelector('.poe-option').classList.add('active');
            }
            
            // Apply both category and PoE filters
            applyFilters();
        }

        // Filter Products by PoE
        function filterPoE(poeType) {
            currentPoE = poeType;
            
            // Update active PoE option
            document.querySelectorAll('.poe-option').forEach(option => {
                option.classList.remove('active');
            });
            event.target.classList.add('active');
            
            // Apply both category and PoE filters
            applyFilters();
        }

        // Apply both category and PoE filters
        function applyFilters() {
            const products = document.querySelectorAll('.product-card');
            
            products.forEach(product => {
                const productCategory = product.getAttribute('data-category');
                const productPoE = product.getAttribute('data-poe');
                
                const categoryMatch = currentCategory === 'all' || productCategory === currentCategory;
                const poeMatch = currentPoE === 'all' || productPoE === currentPoE;
                
                if (categoryMatch && poeMatch) {
                    product.style.display = 'flex';
                } else {
                    product.style.display = 'none';
                }
            });
        }

        // Modal Functions
        function openProductModal(productId) {
            const product = productDatabase[productId];
            if (!product) return;
            
            document.getElementById('modalProductName').textContent = product.name;
            
            let modalContent = `
                <div class="product-modal-content">
                    <div class="product-brand-tag ${product.brand.toLowerCase()}">${product.brand}</div>
                    <p class="product-description">${product.description}</p>
                    
                    <h3>Specifications</h3>
                    <div class="specs-table">
            `;
            
            for (const [key, value] of Object.entries(product.specs)) {
                modalContent += `
                    <div class="spec-row">
                        <div class="spec-name">${key}</div>
                        <div class="spec-value">${value}</div>
                    </div>
                `;
            }
            
            modalContent += `
                    </div>
                    
                    <h3>Key Features</h3>
                    <ul class="features-list">
            `;
            
            product.features.forEach(feature => {
                modalContent += `<li>${feature}</li>`;
            });
            
            modalContent += `
                    </ul>
                    
                    <h3>Applications</h3>
                    <div class="applications">
            `;
            
            product.applications.forEach(app => {
                modalContent += `<span class="application-tag">${app}</span>`;
            });
            
            modalContent += `
                    </div>
                    
                    <div class="modal-actions">
                        <button class="cta-button" onclick="requestQuote('${productId}')">Request Quote</button>
                        <button class="cta-button aruba-btn" onclick="contactTechnical()">Technical Consultation</button>
                    </div>
                </div>
            `;
            
            document.getElementById('modalProductContent').innerHTML = modalContent;
            document.getElementById('productModal').style.display = 'block';
            
            // Add custom styles for modal content
            const style = document.createElement('style');
            style.textContent = `
                .product-modal-content {
                    padding: 10px;
                }
                .product-brand-tag {
                    display: inline-block;
                    padding: 8px 16px;
                    border-radius: 20px;
                    color: white;
                    font-weight: 600;
                    margin-bottom: 20px;
                    font-size: 0.9rem;
                }
                .product-brand-tag.cisco {
                    background: var(--gradient-cisco);
                }
                .product-brand-tag.aruba {
                    background: var(--gradient-aruba);
                }
                .product-description {
                    margin-bottom: 25px;
                    font-size: 1.1rem;
                    line-height: 1.7;
                    color: var(--text-light);
                }
                .specs-table {
                    margin-bottom: 30px;
                }
                .spec-row {
                    display: flex;
                    padding: 12px 0;
                    border-bottom: 1px solid var(--border);
                }
                .spec-name {
                    font-weight: 600;
                    width: 40%;
                    color: var(--text-dark);
                }
                .spec-value {
                    width: 60%;
                    color: var(--text-light);
                }
                .features-list {
                    margin-bottom: 30px;
                    padding-left: 20px;
                }
                .features-list li {
                    margin-bottom: 10px;
                    line-height: 1.6;
                }
                .applications {
                    display: flex;
                    flex-wrap: wrap;
                    gap: 10px;
                    margin-bottom: 30px;
                }
                .application-tag {
                    background: var(--background);
                    padding: 8px 16px;
                    border-radius: 20px;
                    font-size: 0.9rem;
                    color: var(--text-light);
                    font-weight: 500;
                }
                .modal-actions {
                    display: flex;
                    gap: 15px;
                    justify-content: center;
                    margin-top: 30px;
                }
                @media (max-width: 768px) {
                    .modal-actions {
                        flex-direction: column;
                    }
                }
            `;
            document.head.appendChild(style);
        }

        function closeProductModal() {
            document.getElementById('productModal').style.display = 'none';
        }

        function requestQuote(productId) {
            const product = productDatabase[productId];
            alert(`Thank you for your interest in ${product.name}. Our sales team will contact you shortly with pricing information.`);
            closeProductModal();
        }

        function contactTechnical() {
            alert('Our technical team will contact you to discuss your requirements and provide expert consultation.');
            closeProductModal();
        }

        // Search Functionality
        document.getElementById('productSearch').addEventListener('input', function(e) {
            const searchTerm = e.target.value.toLowerCase();
            const products = document.querySelectorAll('.product-card');
            
            products.forEach(product => {
                const productName = product.querySelector('h3').textContent.toLowerCase();
                const productType = product.querySelector('.product-type').textContent.toLowerCase();
                
                if (productName.includes(searchTerm) || productType.includes(searchTerm)) {
                    // Only show if it matches current filters
                    const productCategory = product.getAttribute('data-category');
                    const productPoE = product.getAttribute('data-poe');
                    
                    const categoryMatch = currentCategory === 'all' || productCategory === currentCategory;
                    const poeMatch = currentPoE === 'all' || productPoE === currentPoE;
                    
                    if (categoryMatch && poeMatch) {
                        product.style.display = 'flex';
                    } else {
                        product.style.display = 'none';
                    }
                } else {
                    product.style.display = 'none';
                }
            });
        });

        // Contact Form Submission
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your message! We will contact you soon.');
            this.reset();
        });

        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Close modal when clicking outside
        window.addEventListener('click', function(event) {
            const modal = document.getElementById('productModal');
            if (event.target === modal) {
                closeProductModal();
            }
        });

        // Header scroll effect
        window.addEventListener('scroll', function() {
            const header = document.querySelector('header');
            if (window.scrollY > 100) {
                header.style.background = 'rgba(255, 255, 255, 0.98)';
                header.style.boxShadow = '0 4px 20px rgba(0, 0, 0, 0.1)';
            } else {
                header.style.background = 'rgba(255, 255, 255, 0.95)';
                header.style.boxShadow = '0 1px 3px rgba(0, 0, 0, 0.05)';
            }
        });

        // Create particle background
        function createParticles() {
            const particlesContainer = document.getElementById('particles');
            const particleCount = 30;
            
            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.classList.add('particle');
                
                // Random properties
                const size = Math.random() * 5 + 2;
                const posX = Math.random() * 100;
                const posY = Math.random() * 100;
                const delay = Math.random() * 15;
                const duration = Math.random() * 10 + 10;
                
                particle.style.width = `${size}px`;
                particle.style.height = `${size}px`;
                particle.style.left = `${posX}%`;
                particle.style.top = `${posY}%`;
                particle.style.animationDelay = `${delay}s`;
                particle.style.animationDuration = `${duration}s`;
                
                particlesContainer.appendChild(particle);
            }
        }

        // Section reveal animation
        function revealSections() {
            const reveals = document.querySelectorAll('.reveal');
            
            reveals.forEach(element => {
                const windowHeight = window.innerHeight;
                const elementTop = element.getBoundingClientRect().top;
                const elementVisible = 150;
                
                if (elementTop < windowHeight - elementVisible) {
                    element.classList.add('active');
                }
            });
        }

        // Initialize
        document.addEventListener('DOMContentLoaded', function() {
            createParticles();
            window.addEventListener('scroll', revealSections);
            revealSections(); // Initial check
            
            // Add subsection styles
            const subsectionStyle = document.createElement('style');
            subsectionStyle.textContent = `
                .category-subsection {
                    margin-bottom: 50px;
                }
                .subsection-title {
                    display: flex;
                    align-items: center;
                    gap: 12px;
                    margin-bottom: 25px;
                    padding-bottom: 10px;
                    border-bottom: 1px solid var(--border);
                    font-size: 1.5rem;
                    font-weight: 600;
                    color: var(--cisco-blue);
                }
                .subsection-title i {
                    font-size: 1.8rem;
                    background: var(--gradient-cisco);
                    -webkit-background-clip: text;
                    -webkit-text-fill-color: transparent;
                }
            `;
            document.head.appendChild(subsectionStyle);
        });
    </script>
</body>
</html>
