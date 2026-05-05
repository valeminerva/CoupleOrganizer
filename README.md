# CoupleOrganizer
<!DOCTYPE html>
<html>
<head>
  <title>Our Home Hub</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      padding: 20px;
      background: #f5f5f5;
    }

    h1 {
      font-size: 28px;
    }

    .card {
      background: white;
      padding: 15px;
      margin: 10px 0;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }

    input {
      padding: 8px;
      margin-right: 5px;
    }

    button {
      padding: 8px 12px;
      background: black;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    li {
      margin: 5px 0;
    }
  </style>
</head>
<body>

<h1>Our Home Hub</h1>

<div class="card">
  <h2>Activities</h2>
  <input id="activityInput" placeholder="Add activity">
  <button onclick="addActivity()">Add</button>
  <ul id="activityList"></ul>
</div>

<div class="card">
  <h2>Grocery List</h2>
  <input id="groceryInput" placeholder="Add item">
  <button onclick="addGrocery()">Add</button>
  <ul id="groceryList"></ul>
</div>

<div class="card">
  <h2>Chores</h2>
  <input id="choreInput" placeholder="Add chore">
  <button onclick="addChore()">Add</button>
  <ul id="choreList"></ul>
</div>

<script>
function addActivity() {
  const input = document.getElementById("activityInput");
  const list = document.getElementById("activityList");

  if (input.value.trim() === "") return;

  const li = document.createElement("li");
  li.textContent = input.value;

  list.appendChild(li);
  input.value = "";
}

function addGrocery() {
  const input = document.getElementById("groceryInput");
  const list = document.getElementById("groceryList");

  if (input.value.trim() === "") return;

  const li = document.createElement("li");
  li.textContent = input.value;

  list.appendChild(li);
  input.value = "";
}

function addChore() {
  const input = document.getElementById("choreInput");
  const list = document.getElementById("choreList");

  if (input.value.trim() === "") return;

  const li = document.createElement("li");
  li.textContent = input.value;

  list.appendChild(li);
  input.value = "";
}
</script>

</body>
</html>
