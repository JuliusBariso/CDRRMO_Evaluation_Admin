[CDRRMO_peer evaluation_(admin_staff).html](https://github.com/user-attachments/files/27950695/CDRRMO_peer.evaluation_.admin_staff.html)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CDRRMO Peer Evaluation Form</title>
    <style>
        :root {
            --primary-color: #0284c7;
            --primary-dark: #0369a1;
            --bg-color: #f8fafc;
            --card-bg: #ffffff;
            --text-main: #0f172a;
            --text-muted: #475569;
            --border-color: #cbd5e1;
            --row-alt: #f1f5f9;
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Arial, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
            padding: 16px;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            background: var(--card-bg);
            padding: 24px;
            border-radius: 12px;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
        }

        .header {
            text-align: center;
            margin-bottom: 24px;
            border-bottom: 3px solid var(--primary-color);
            padding-bottom: 16px;
        }

        .header h1 { font-size: 1.6rem; color: var(--primary-dark); text-transform: uppercase; letter-spacing: 0.5px; }
        .header h2 { font-size: 1.2rem; color: var(--text-muted); font-weight: 500; margin-top: 4px; }

        .meta-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 16px;
            margin-bottom: 24px;
            background: var(--bg-color);
            padding: 16px;
            border-radius: 8px;
            border: 1px solid var(--border-color);
        }

        .form-group {
            display: flex;
            flex-direction: column;
        }

        .form-group label {
            font-weight: 600;
            font-size: 0.9rem;
            margin-bottom: 6px;
            color: var(--text-muted);
        }

        .form-group input[type="text"], .form-group input[type="date"], .form-group input[type="email"] {
            padding: 10px;
            border: 1px solid var(--border-color);
            border-radius: 6px;
            font-size: 1rem;
            background: #fff;
        }

        .scale-box {
            background: #f0fdf4;
            border: 1px solid #bbf7d0;
            color: #166534;
            padding: 12px;
            border-radius: 8px;
            margin-bottom: 24px;
            font-size: 0.95rem;
            text-align: center;
        }

        .section-title {
            background: var(--primary-color);
            color: white;
            padding: 8px 14px;
            font-size: 1.1rem;
            border-radius: 6px;
            margin: 28px 0 14px 0;
            text-transform: uppercase;
        }

        /* Desktop Table View Styles */
        .matrix-table {
            width: 100%;
            border-collapse: collapse;
            margin-bottom: 16px;
        }

        .matrix-table th, .matrix-table td {
            padding: 12px;
            border-bottom: 1px solid var(--border-color);
            text-align: left;
        }

        .matrix-table th {
            background-color: var(--bg-color);
            font-weight: 600;
            color: var(--text-muted);
        }

        .matrix-table td.radio-cell {
            text-align: center;
            width: 60px;
        }

        .matrix-table tr:nth-child(even) {
            background-color: #fafafa;
        }

        input[type="radio"] {
            width: 20px;
            height: 20px;
            cursor: pointer;
            accent-color: var(--primary-color);
        }

        /* Mobile Layout Card Elements */
        .mobile-question-card {
            display: none;
        }

        textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid var(--border-color);
            border-radius: 6px;
            font-size: 1rem;
            resize: vertical;
            font-family: inherit;
        }

        button {
            display: block;
            width: 100%;
            background-color: var(--primary-color);
            color: white;
            border: none;
            padding: 14px;
            font-size: 1.1rem;
            font-weight: 700;
            border-radius: 8px;
            cursor: pointer;
            margin-top: 30px;
            transition: background 0.2s;
            box-shadow: 0 4px 6px -1px rgba(2, 132, 199, 0.4);
        }

        button:hover { background-color: var(--primary-dark); }

        @media (max-width: 650px) {
            .meta-grid { grid-template-columns: 1fr; }
            .matrix-table { display: none; }
            
            .mobile-question-card {
                display: block;
                background: #fff;
                border: 1px solid var(--border-color);
                border-radius: 8px;
                padding: 14px;
                margin-bottom: 14px;
            }

            .mobile-question-text {
                font-weight: 600;
                margin-bottom: 12px;
                font-size: 1rem;
            }

            .mobile-radio-options {
                display: flex;
                justify-content: space-between;
                align-items: center;
                background: var(--bg-color);
                padding: 10px;
                border-radius: 6px;
            }

            .mobile-option {
                display: flex;
                flex-direction: column;
                align-items: center;
                gap: 4px;
                font-size: 0.85rem;
                font-weight: 600;
                color: var(--text-muted);
            }
        }
    </style>
</head>
<body>

<div class="container">
    <div class="header">
        <h1>CDRRMO Peer Evaluation Form</h1>
        <h2>Administrative Staff</h2>
    </div>

    <form id="evaluationForm">
        
        <!-- Target Recipient Email Configuration Field -->
        <div class="form-group" style="margin-bottom: 20px;">
            <label for="submissionEmail">Designated Recipient Email:</label>
            <input type="email" id="submissionEmail" value="gelmolatojunior@gmail.com" required>
        </div>

        <div class="meta-grid">
            <div class="form-group">
                <label for="empName">Name of Employee Being Evaluated</label>
                <input type="text" id="empName" required>
            </div>
            <div class="form-group">
                <label for="position">Position</label>
                <input type="text" id="position" required>
            </div>
            <div class="form-group">
                <label for="office">Office/Unit</label>
                <input type="text" id="office" value="CDRRMO" required>
            </div>
            <div class="form-group">
                <label for="evalDate">Date</label>
                <input type="date" id="evalDate" required>
            </div>
        </div>

        <div class="scale-box">
            <strong>Rating Scale:</strong> 5 – Outstanding | 4 – Very Satisfactory | 3 – Satisfactory | 2 – Needs Improvement | 1 – Poor
        </div>

        <!-- Dynamic Form Target Container Block -->
        <div id="dynamicSections"></div>

        <!-- Section VI: Comments -->
        <div class="section-title">VI. Areas for Improvement and Additional Comments</div>
        <div class="form-group">
            <textarea id="comments" rows="5" placeholder="Provide precise evaluation notes or structural feedback here..."></textarea>
        </div>

        <!-- Evaluator Context Grid -->
        <div class="section-title">Evaluator Information</div>
        <div class="meta-grid">
            <div class="form-group">
                <label for="evaluatorName">Evaluator's Name (Optional)</label>
                <input type="text" id="evaluatorName" placeholder="Anonymous">
            </div>
            <div class="form-group">
                <label for="submissionDate">Current Date</label>
                <input type="date" id="submissionDate" required>
            </div>
        </div>

        <button type="submit">Submit and Generate Email Report</button>
    </form>
</div>

<script>
    // System Form Parameters Object Array Matrix Schema
    const formSchema = [
        {
            title: "I. Work Performance",
            key: "WP",
            questions: [
                { id: 1, text: "Completes assigned tasks on time" },
                { id: 2, text: "Accuracy of work output" },
                { id: 3, text: "Organizes documents and records properly" },
                { id: 4, text: "Follows office procedures and guidelines" },
                { id: 5, text: "Shows initiative in accomplishing tasks" }
            ]
        },
        {
            title: "II. Teamwork & Cooperation",
            key: "TC",
            questions: [
                { id: 6, text: "Cooperates with co-workers" },
                { id: 7, text: "Willingness to assist others" },
                { id: 8, text: "Maintains positive working relationships" },
                { id: 9, text: "Respects opinions of others" },
                { id: 10, text: "Supports team objectives" }
            ]
        },
        {
            title: "III. Communication",
            key: "CM",
            questions: [
                { id: 11, text: "Communicates clearly with staff" },
                { id: 12, text: "Responds promptly to requests" },
                { id: 13, text: "Maintains professionalism in communication" },
                { id: 14, text: "Shares important information with team" }
            ]
        },
        {
            title: "IV. Professionalism & Work Ethics",
            key: "PW",
            questions: [
                { id: 15, text: "Reports to work on time" },
                { id: 16, text: "Demonstrates reliability" },
                { id: 17, text: "Maintains confidentiality of documents" },
                { id: 18, text: "Respond to emergency calls if needed" },
                { id: 19, text: "Displays proper conduct in the workplace" }
            ]
        },
        {
            title: "V. Customer Service",
            key: "CS",
            questions: [
                { id: 20, text: "Courteous to clients" },
                { id: 21, text: "Handles requests efficiently" },
                { id: 22, text: "Provides accurate information" },
                { id: 23, text: "Demonstrates helpful attitude" }
            ]
        }
    ];

    // Standard SPMS Evaluation Scale Conversion Matrix Function
    function getDescriptiveRating(score) {
        if (score === 0) return "Incomplete";
        if (score >= 4.50) return "Outstanding";
        if (score >= 3.50) return "Very Satisfactory";
        if (score >= 2.50) return "Satisfactory";
        if (score >= 1.50) return "Needs Improvement";
        return "Poor";
    }

    // Set Default Calendar dates to today
    const today = new Date().toISOString().split('T')[0];
    document.getElementById('evalDate').value = today;
    document.getElementById('submissionDate').value = today;

    const targetContainer = document.getElementById('dynamicSections');

    // Build Responsive DOM layout elements loop
    formSchema.forEach(section => {
        let sectionHTML = `<div class="section-title">${section.title}</div>`;
        
        // Desktop matrix elements layout
        sectionHTML += `<table class="matrix-table">
            <thead>
                <tr>
                    <th>Evaluation Criteria</th>
                    <th style="text-align:center">1</th>
                    <th style="text-align:center">2</th>
                    <th style="text-align:center">3</th>
                    <th style="text-align:center">4</th>
                    <th style="text-align:center">5</th>
                </tr>
            </thead>
            <tbody>`;

        section.questions.forEach(q => {
            sectionHTML += `<tr>
                <td>${q.id}. ${q.text}</td>`;
                for(let i=1; i<=5; i++) {
                    sectionHTML += `<td class="radio-cell">
                        <input type="radio" name="q_${q.id}" value="${i}" data-text="${q.text}" required>
                    </td>`;
                }
            sectionHTML += `</tr>`;
        });
        sectionHTML += `</tbody></table>`;

        // Mobile layout cards components
        section.questions.forEach(q => {
            sectionHTML += `<div class="mobile-question-card">
                <div class="mobile-question-text">${q.id}. ${q.text}</div>
                <div class="mobile-radio-options">`;
                for(let i=1; i<=5; i++) {
                    sectionHTML += `<label class="mobile-option">
                        <span>${i}</span>
                        <input type="radio" name="m_q_${q.id}" value="${i}" data-sync="q_${q.id}">
                    </label>`;
                }
            sectionHTML += `</div></div>`;
        });

        targetContainer.innerHTML += sectionHTML;
    });

    // Cross-Synchronization Interactivity Layer Engine between view screens
    document.addEventListener('change', function(e) {
        if(e.target.name.startsWith('q_')) {
            const targetMobileName = 'm_q_' + e.target.name.split('_')[1];
            const mobileRadio = document.querySelector(`input[name="${targetMobileName}"][value="${e.target.value}"]`);
            if(mobileRadio) mobileRadio.checked = true;
        }
        if(e.target.name.startsWith('m_q_')) {
            const targetDesktopName = 'q_' + e.target.name.split('_')[2];
            const desktopRadio = document.querySelector(`input[name="${targetDesktopName}"][value="${e.target.value}"]`);
            if(desktopRadio) {
                desktopRadio.checked = true;
                desktopRadio.setCustomValidity(""); 
            }
        }
    });

    // Data parsing structure compiler on Form submission execution
    document.getElementById('evaluationForm').addEventListener('submit', function(e) {
        e.preventDefault();

        const sendTo = document.getElementById('submissionEmail').value;
        const targetEmp = document.getElementById('empName').value;
        const targetPos = document.getElementById('position').value;
        const targetOffice = document.getElementById('office').value;
        const targetDate = document.getElementById('evalDate').value;
        const commentsText = document.getElementById('comments').value || 'None provided';
        const evaluator = document.getElementById('evaluatorName').value || 'Anonymous';
        const rawSubDate = document.getElementById('submissionDate').value;

        let totalScoreSum = 0;
        let countedQuestions = 0;

        // Perform calculation dynamically at the moment of submission
        formSchema.forEach(section => {
            section.questions.forEach(q => {
                const checkedRadio = document.querySelector(`input[name="q_${q.id}"]:checked`);
                if (checkedRadio) {
                    totalScoreSum += parseFloat(checkedRadio.value);
                    countedQuestions++;
                }
            });
        });

        const finalAverageScore = countedQuestions > 0 ? (totalScoreSum / countedQuestions) : 0;
        const finalPercentageScore = finalAverageScore > 0 ? ((finalAverageScore / 5) * 100) : 0;
        const finalDescriptiveRating = getDescriptiveRating(finalAverageScore);

        // Build Structured plain-text email string output with ratings written directly in the header
        let trackingBody = `CDRRMO PEER PERFORMANCE EVALUATION REPORT\n`;
        trackingBody += `==================================================\n`;
        trackingBody += `OVERALL SCORE RATING      : ${finalAverageScore.toFixed(2)} / 5.00 (${Math.round(finalPercentageScore)}%)\n`;
        trackingBody += `OVERALL ADJECTIVAL RATING : ${finalDescriptiveRating}\n`;
        trackingBody += `==================================================\n\n`;
        
        trackingBody += `EMPLOYEE UNDER EVALUATION : ${targetEmp}\n`;
        trackingBody += `POSITION                  : ${targetPos}\n`;
        trackingBody += `OFFICE/UNIT               : ${targetOffice}\n`;
        trackingBody += `DATE ASSESSED             : ${targetDate}\n\n`;
        
        trackingBody += `==================================================\n`;
        trackingBody += `CRITERIA RUNNING SCORES LOG:\n`;
        trackingBody += `==================================================\n\n`;

        formSchema.forEach(section => {
            trackingBody += `--- ${section.title} ---\n`;
            section.questions.forEach(q => {
                const selectedVal = document.querySelector(`input[name="q_${q.id}"]:checked`).value;
                trackingBody += `Question ${q.id}: [Score: ${selectedVal}] - ${q.text}\n`;
            });
            trackingBody += `\n`;
        });

        trackingBody += `==================================================\n`;
        trackingBody += `VI. AREAS FOR IMPROVEMENT & EXTRA EVALUATOR COMMENTS:\n`;
        trackingBody += `==================================================\n`;
        trackingBody += `${commentsText}\n\n`;
        
        trackingBody += `==================================================\n`;
        trackingBody += `SUBMISSION METADATA:\n`;
        trackingBody += `==================================================\n`;
        trackingBody += `Evaluator: ${evaluator}\n`;
        trackingBody += `Report Compiled on: ${rawSubDate}\n`;

        const subjectLine = `Peer Eval [Score: ${finalAverageScore.toFixed(2)} - ${finalDescriptiveRating}] - ${targetEmp}`;

        // Launch user mail client with payload strings
        window.location.href = `mailto:${sendTo}?subject=${encodeURIComponent(subjectLine)}&body=${encodeURIComponent(trackingBody)}`;
    });
</script>

</body>
</html>
