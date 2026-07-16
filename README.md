/* General Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: #333;
    background-color: #f5f5f5;
}

a {
    color: #0066cc;
    text-decoration: none;
}

a:hover {
    text-decoration: underline;
}

/* CV Container */
.cv-container {
    max-width: 900px;
    margin: 20px auto;
    background-color: #fff;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    overflow: hidden;
}

/* CV Header */
.cv-header {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 40px 30px;
    text-align: center;
}

.cv-header h1 {
    font-size: 2.5em;
    margin-bottom: 10px;
    letter-spacing: 2px;
}

.job-title {
    font-size: 1.3em;
    margin-bottom: 20px;
    opacity: 0.9;
}

.contact-info {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
    font-size: 0.9em;
    margin-top: 15px;
}

.contact-info a {
    color: #fff;
    text-decoration: underline;
}

.contact-info a:hover {
    opacity: 0.8;
}

/* CV Navigation */
.cv-nav {
    padding: 15px 30px;
    background-color: #f9f9f9;
    border-bottom: 1px solid #eee;
}

.cv-nav a {
    display: inline-block;
    color: #0066cc;
    font-weight: 500;
    padding: 8px 15px;
    border: 1px solid #0066cc;
    border-radius: 4px;
    transition: all 0.3s ease;
}

.cv-nav a:hover {
    background-color: #0066cc;
    color: white;
    text-decoration: none;
}

/* CV Content */
.cv-content {
    padding: 40px 30px;
}

/* Section Styles */
.cv-section {
    margin-bottom: 30px;
    border-bottom: 2px solid #eee;
    padding-bottom: 25px;
}

.cv-section:last-of-type {
    border-bottom: none;
}

.section-title {
    font-size: 1.5em;
    color: #667eea;
    margin-bottom: 20px;
    padding-bottom: 10px;
    border-bottom: 3px solid #667eea;
    display: inline-block;
}

/* Job Entry Styles */
.job-entry {
    margin-bottom: 25px;
}

.job-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 8px;
}

.job-header h3 {
    font-size: 1.2em;
    color: #333;
}

.date {
    color: #999;
    font-size: 0.9em;
    font-style: italic;
}

.company {
    color: #666;
    font-weight: bold;
    margin-bottom: 10px;
}

.job-entry ul {
    list-style-position: inside;
    color: #555;
}

.job-entry ul li {
    margin-bottom: 8px;
    line-height: 1.5;
}

/* Education Entry Styles */
.education-entry {
    margin-bottom: 20px;
}

.edu-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 8px;
}

.edu-header h3 {
    font-size: 1.1em;
    color: #333;
}

.institution {
    color: #666;
    font-weight: bold;
    margin-bottom: 5px;
}

.gpa {
    color: #999;
    font-size: 0.9em;
}

/* Skills Grid */
.skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}

.skill-category {
    padding: 15px;
    background-color: #f9f9f9;
    border-left: 4px solid #667eea;
    border-radius: 4px;
}

.skill-category h4 {
    color: #667eea;
    margin-bottom: 10px;
}

.skill-category p {
    color: #555;
    line-height: 1.5;
}

/* Project Entry Styles */
.project-entry {
    margin-bottom: 20px;
    padding: 15px;
    background-color: #f9f9f9;
    border-left: 4px solid #764ba2;
    border-radius: 4px;
}

.project-entry h3 {
    color: #333;
    margin-bottom: 8px;
}

.project-date {
    color: #999;
    font-size: 0.9em;
    margin-bottom: 10px;
}

.project-link {
    margin-top: 10px;
}

.project-link a {
    color: #764ba2;
    font-weight: bold;
}

/* CV Footer */
.cv-footer {
    background-color: #f9f9f9;
    padding: 20px 30px;
    text-align: center;
    color: #999;
    font-size: 0.9em;
    border-top: 1px solid #eee;
}

/* Print Styles */
@media print {
    body {
        background-color: white;
    }
    
    .cv-container {
        max-width: 100%;
        margin: 0;
        box-shadow: none;
        border-radius: 0;
    }
    
    .cv-nav {
        display: none;
    }
    
    .cv-footer {
        display: none;
    }
}

/* Responsive Design */
@media (max-width: 768px) {
    .cv-header {
        padding: 30px 20px;
    }
    
    .cv-header h1 {
        font-size: 2em;
    }
    
    .contact-info {
        flex-direction: column;
        gap: 10px;
    }
    
    .cv-content {
        padding: 20px;
    }
    
    .job-header,
    .edu-header {
        flex-direction: column;
        align-items: flex-start;
        gap: 5px;
    }
    
    .skills-grid {
        grid-template-columns: 1fr;
    }
}
