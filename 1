<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Prop Firm Calculator</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
      background: #f5f5f5;
      margin: 0;
      padding: 20px;
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .calculator-container {
      width: 100%;
      max-width: 640px;
      background: #2d2d2d;
      border-radius: 12px;
      overflow: hidden;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
    }

    .calculator-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 1px;
      background: #1a1a1a;
      padding: 1px;
    }

    .section {
      background: #2d2d2d;
      padding: 16px;
    }

    .section-title {
      font-size: 10px;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 1.2px;
      color: #808080;
      margin-bottom: 14px;
    }

    .row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 8px 0;
      border-bottom: 1px solid #3a3a3a;
    }

    .row:last-child {
      border-bottom: none;
    }

    .label {
      font-size: 12px;
      color: #b0b0b0;
      font-weight: 500;
    }

    .value {
      font-size: 13px;
      font-weight: 600;
      padding: 5px 10px;
      border-radius: 6px;
      background: #1a1a1a;
    }

    .value.positive {
      color: #4ade80;
    }

    .value.negative {
      color: #ef4444;
    }

    .value.neutral {
      color: #fbbf24;
    }

    input {
      width: 100px;
      padding: 5px 10px;
      font-size: 13px;
      font-weight: 600;
      background: #1a1a1a;
      border: 1px solid #404040;
      border-radius: 6px;
      color: #ffffff;
      text-align: right;
      transition: all 0.2s ease;
    }

    input:hover {
      border-color: #505050;
    }

    input:focus {
      outline: none;
      border-color: #4ade80;
      background: #222;
    }

    .monthly-income-row {
      grid-column: span 2;
      background: #2d2d2d;
      padding: 12px 16px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-top: 1px solid #3a3a3a;
    }

    .monthly-income-row .label {
      font-size: 12px;
      font-weight: 600;
      color: #b0b0b0;
      text-transform: uppercase;
      letter-spacing: 0.5px;
    }

    .monthly-income-row .value {
      font-size: 16px;
      font-weight: 700;
      color: #4ade80;
      background: rgba(74, 222, 128, 0.1);
      padding: 6px 12px;
      border-radius: 8px;
    }

    /* Special styling for ROI and Profit rows */
    .row.highlight .value {
      background: #222;
    }

    @media (max-width: 600px) {
      body {
        padding: 10px;
      }
      
      .calculator-grid {
        grid-template-columns: 1fr;
      }

      .monthly-income-row {
        grid-column: span 1;
      }

      input {
        width: 90px;
      }
    }

    /* Ensure it works well in iframe */
    html, body {
      height: auto;
      min-height: auto;
    }

    @media (max-width: 500px) {
      body {
        padding: 5px;
      }
      
      .calculator-container {
        max-width: 100%;
      }
    }
  </style>
</head>

<body>
  <div class="calculator-container">
    <div class="calculator-grid">
      <!-- Results Section -->
      <div class="section">
        <div class="section-title">Results</div>
        <div class="row">
          <span class="label">Total Evaluations</span>
          <span class="value neutral" id="totalEvaluations">5</span>
        </div>
        <div class="row">
          <span class="label">Funded Accounts</span>
          <span class="value neutral" id="totalFundedAccounts">3</span>
        </div>
        <div class="row">
          <span class="label">Total Expenses</span>
          <span class="value negative" id="totalExpenses">$385.00</span>
        </div>
        <div class="row">
          <span class="label">Total Payout</span>
          <span class="value positive" id="totalPayoutAmount">$3,600.00</span>
        </div>
        <div class="row highlight">
          <span class="label">Profit</span>
          <span class="value" id="profit">$3,215.00</span>
        </div>
        <div class="row highlight">
          <span class="label">ROI</span>
          <span class="value" id="roi">835%</span>
        </div>
      </div>

      <!-- Database Section -->
      <div class="section">
        <div class="section-title">Configuration</div>
        <div class="row">
          <span class="label">Total Evaluations</span>
          <input type="number" id="dbTotalEvaluations" value="5" min="0">
        </div>
        <div class="row">
          <span class="label">Funded Rate</span>
          <input type="text" id="dbFundedRate" value="67%">
        </div>
        <div class="row">
          <span class="label">Payout Rate</span>
          <input type="text" id="dbPayoutRate" value="100%">
        </div>
        <div class="row">
          <span class="label">Cost Per Eval</span>
          <input type="text" id="dbCostPerEval" value="$77">
        </div>
        <div class="row">
          <span class="label">Cost Per Funded</span>
          <input type="text" id="dbCostPerFunded" value="$0">
        </div>
        <div class="row">
          <span class="label">Avg Payout</span>
          <input type="text" id="dbAvgPayout" value="$1,200">
        </div>
        <div class="row">
          <span class="label">Per Payout</span>
          <input type="text" id="dbPerPayout" value="$1,200">
        </div>
      </div>

      <!-- Monthly Income Row -->
      <div class="monthly-income-row">
        <span class="label">Monthly Income Potential</span>
        <span class="value" id="monthlyIncome">$7,200.00</span>
      </div>
    </div>
  </div>

  <script>
    // Helper functions to parse currency and percentage inputs
    function parseCurrency(value) {
      if (typeof value === 'number') return value;
      return parseFloat(value.replace(/[$,]/g, '')) || 0;
    }

    function parsePercentage(value) {
      if (typeof value === 'number') return value / 100;
      return parseFloat(value.replace('%', '')) / 100 || 0;
    }

    function formatCurrency(value) {
      return new Intl.NumberFormat('en-US', {
        style: 'currency',
        currency: 'USD',
        minimumFractionDigits: 2,
        maximumFractionDigits: 2
      }).format(value);
    }

    function formatPercentage(value) {
      return Math.round(value * 100) + '%';
    }
    
    // Calculate and update all results
    function calculateResults() {
      // Get database values
      const totalEvals = parseFloat(document.getElementById('dbTotalEvaluations').value) || 0;
      const fundedRate = parsePercentage(document.getElementById('dbFundedRate').value);
      const payoutRate = parsePercentage(document.getElementById('dbPayoutRate').value);
      const costPerEval = parseCurrency(document.getElementById('dbCostPerEval').value);
      const costPerFunded = parseCurrency(document.getElementById('dbCostPerFunded').value);
      const avgPayout = parseCurrency(document.getElementById('dbAvgPayout').value);
      const perPayout = parseCurrency(document.getElementById('dbPerPayout').value);
      
      // Calculate results
      const totalFundedAccounts = Math.round(totalEvals * fundedRate);
      const totalExpenses = totalEvals * costPerEval;
      const totalPayoutAmount = totalFundedAccounts * avgPayout;
      const profit = totalPayoutAmount - totalExpenses;
      const roi = totalExpenses > 0 ? (profit / totalExpenses) : 0;
      const monthlyIncome = totalFundedAccounts * perPayout * 2; // 2 payouts per month
      
      // Update results display
      document.getElementById('totalEvaluations').textContent = totalEvals;
      document.getElementById('totalFundedAccounts').textContent = totalFundedAccounts;
      document.getElementById('totalExpenses').textContent = formatCurrency(totalExpenses);
      document.getElementById('totalPayoutAmount').textContent = formatCurrency(totalPayoutAmount);
      document.getElementById('profit').textContent = formatCurrency(profit);
      document.getElementById('roi').textContent = formatPercentage(roi);
      document.getElementById('monthlyIncome').textContent = formatCurrency(monthlyIncome);
      
      // Update colors based on values
      const profitElement = document.getElementById('profit');
      const roiElement = document.getElementById('roi');
      if (profit < 0) {
        profitElement.className = 'value negative';
        roiElement.className = 'value negative';
      } else {
        profitElement.className = 'value positive';
        roiElement.className = 'value positive';
      }
    }
    
    // Add event listeners to all database inputs
    document.getElementById('dbTotalEvaluations').addEventListener('input', calculateResults);
    document.getElementById('dbFundedRate').addEventListener('input', calculateResults);
    document.getElementById('dbPayoutRate').addEventListener('input', calculateResults);
    document.getElementById('dbCostPerEval').addEventListener('input', calculateResults);
    document.getElementById('dbCostPerFunded').addEventListener('input', calculateResults);
    document.getElementById('dbAvgPayout').addEventListener('input', calculateResults);
    document.getElementById('dbPerPayout').addEventListener('input', calculateResults);
    
    // Format currency inputs on blur
    const currencyInputs = ['dbCostPerEval', 'dbCostPerFunded', 'dbAvgPayout', 'dbPerPayout'];
    currencyInputs.forEach(id => {
      document.getElementById(id).addEventListener('blur', function() {
        const value = parseCurrency(this.value);
        if (!isNaN(value)) {
          this.value = formatCurrency(value);
        }
      });
    });
    
    // Format percentage inputs on blur
    const percentInputs = ['dbFundedRate', 'dbPayoutRate'];
    percentInputs.forEach(id => {
      document.getElementById(id).addEventListener('blur', function() {
        const value = parsePercentage(this.value);
        if (!isNaN(value)) {
          this.value = formatPercentage(value);
        }
      });
    });
    
    // Initial calculation
    calculateResults();
  </script>
</body>

</html>
