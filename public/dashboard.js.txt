fetch('/api/students')
  .then(response => response.json())
  .then(data => {
    const container = document.getElementById('student-data');
    container.innerHTML = JSON.stringify(data, null, 2);
  })
  .catch(err => console.error(err));
