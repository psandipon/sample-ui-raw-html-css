<template>
  <div class="row">
    <div class="side">
      <h3>account panel</h3>
      <ul>
        <li><a href="#0">overview</a></li>
        <li><a href="#0">messages</a></li>
        <li><a href="#0">clients</a></li>
        <li style="padding-top:30px"><a href="#0">logout</a></li>
      </ul>
    </div>
    <div class="main">
      <h3>MESSAGES</h3>
      <p>Use this messaging</p>

      <header class="table-header">
        <p class="table-title" style="">
          MESSAGES
        </p>
        <button class="table-action" style=" flex: 5%;">...</button>
      </header>

      <table>
        <tr>
          <td>
            <div class="circle">
              <p>8</p>
            </div>
            <div class="circle-text">
              <p>10:58</p>
            </div>
          </td>
          <td class="msg">
            <h4 class="msg-title">Emmanuel</h4>
            <h5 class="msg-body">
              Hello, I am your doctor. How are you doing at the moment ? Do you
              have any question about your treatment ?
            </h5>
          </td>
        </tr>
        <tr>
          <td>
            <div class="circle">
              <p>8</p>
            </div>
            <div class="circle-text">
              <p>10:58</p>
            </div>
          </td>
          <td class="msg">
            <h4 class="msg-title">Paul Stdu</h4>
            <h5 class="msg-body">
              I am good doc. I do have a question yes. I take finasteride since
              January of this year. You have any idea when I can ...
            </h5>
          </td>
        </tr>
        <tr>
          <td>
            <div class="circle">
              <p>8</p>
            </div>
            <div class="circle-text">
              <p>10:58</p>
            </div>
          </td>
          <td class="msg">
            <h4 class="msg-title">Donald Trump</h4>
            <h5 class="msg-body">
              Generally, results start appearing at month 3. From that moment,
              the rate at which you lose your hair decreases ...
            </h5>
          </td>
        </tr>
        <tr>
          <td>
            <div class="circle-text">
              <p>10:58</p>
            </div>
          </td>
          <td class="msg">
            <h4 class="msg-title">Barrak Obama</h4>
            <h5 class="msg-body">
              Thank you
            </h5>
          </td>
        </tr>
        <tr>
          <td>
            <div class="circle-text">
              <p>22 MAR</p>
            </div>
          </td>
          <td class="msg">
            <h4 class="msg-title">Joe Biden</h4>
            <h5 class="msg-body">
              Thanks joe
            </h5>
          </td>
        </tr>
        <tr>
          <td>
            <div class="circle-text">
              <p>22 MAR</p>
            </div>
          </td>
          <td class="msg">
            <h4 class="msg-title">God Himself</h4>
            <h5 class="msg-body">
              Ok Doctor. No questions for now, but will reach out once i have
              any. Have a good day.
            </h5>
          </td>
        </tr>
      </table>

      <div class="card">
        <div class="container">
          <p>CLICK THE ICON ON THE RIGHT TO START A NEW MESSAGE</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.row {
  text-align: left;
  display: flex;
  list-style-type: none;
  margin-left: 100px;
  margin-right: 100px;
}

.side {
  flex: 20%;
  background-color: white;
  margin: 20px;
  h3 {
    text-transform: uppercase;
  }
  ul {
    list-style: none;
    margin: 0;
    padding: 0;
    margin-top: 60px;
  }
  a {
    text-transform: capitalize;
    text-decoration: none;
    color: grey;
    padding-top: 15px;
    padding-bottom: 15px;
    display: inline-block;
  }

  a:hover {
    font-weight: bold;
    color: #000000;
  }
}

.main {
  flex: 80%;
  background-color: white;
  margin: 20px;
  h3 {
    text-transform: uppercase;
  }

  ul {
    list-style: none;
    margin: 0;
    padding: 0;
    margin-top: 60px;
  }

  a {
    text-transform: capitalize;
    text-decoration: none;
    color: grey;
    padding-top: 15px;
    padding-bottom: 15px;
    display: inline-block;
  }

  a:hover {
    font-weight: bold;
    color: #000000;
  }

  table,
  td,
  th {
    border-top: 1px solid #ddd;
    border-bottom: 1px solid #ddd;
    text-align: left;
  }

  table {
    border-collapse: collapse;
    width: 100%;
  }

  th,
  td {
    padding: 15px;
  }

  tr td:first-child {
    width: 8em;
    min-width: 8em;
    max-width: 8em;
    word-break: break-all;
  }

  .card {
    box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.2);
    transition: 0.3s;
  }

  .card:hover {
    box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
  }

  .container {
    padding: 2px 16px;
  }
}

.circle {
  height: 24px;
  width: 24px;
  background-color: #555;
  border-radius: 50%;
  margin-top: -10px;
  p {
    color: white;
    padding-top: 5px;
    margin-left: 9px;
    font-size: 12px;
  }
}

.circle-text {
  p {
    margin: 0px !important;
    padding-top: 5px;
  }
}

.msg {
  .msg-title {
    padding: 0 !important;
    margin-top: 5px;
    margin-bottom: 8px;
    color: black;
  }
  .msg-body {
    margin: 0 !important;
    padding: 0 !important;
    color: gray;
    overflow: hidden;
    max-width: 600px;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }
}

.table-header {
  display: flex;
  border-top: 1px solid black;
  margin-top: 0px;
  .table-title {
    color: black;
    font-weight: 700;
    flex: 95%;
    text-align: center;
    margin-top: 20px;
  }
  .table-action {
    background-color: #ffffff00;
    border: none;
    color: black;
    padding: 15px 32px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    margin: 4px 2px;
    cursor: pointer;
    font-weight: 700;
    letter-spacing: 2px;
  }
}
</style>
