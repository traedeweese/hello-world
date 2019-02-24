<style>
  h1 {
  text-align: center;
}
p {
  text-align: center;
  font-size: 20px;
}
body {
  background: green;
  text-align: left;
}
#form-outer {
  background-color: rgb(250, 250, 250);
  margin: 0 auto;
  border-radius: 4px;
  width: 75%;
  max-width: 900px;
  padding: 10px;
  padding-top: 20px;
}
.labels {
  display: inline-block;
  text-align: right;
  width: 40%;
  padding: 5px;
  vertical-align: top;
  margin-top: 10px;
}
.rightTab {
  display: inline-block;
  text-align: left;
  width: 48%;
  vertical-align: middle;
}
.input-field {
  height: 20px;
  width: 280px;
  padding: 5px;
  margin: 10px;
  border: 1px solid #c0c0c0;
  border-radius: 2px;
}
.dropdown {
  height: 35px;
  width: 140px;
  padding: 5px;
  margin: 10px;  
  margin-top: 15px;
  border: 1px solid #c0c0c0;
  border-radius: 2px;
}
.radio, .checkbox {
  position: relative;
  left: -43px;
  margin-left: 10px;
  display: block;
  padding-bottom: 10px;
}
.userRatings,
input[type="checkbox"] {
  float: left;
  margin-right: 5px;
}
#submit {
  background-color: #59ace0;
  border-radius: 4px;
  color: white;
  font-size: 1em;
  height: 40px;
  width: 96px;
  margin: 10px;
  border: 0px solid;
}
  </style>
<script src="https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js"></script>

<h1 id="title">How am I doing as a husband and father?</h1>
<div id="form-outer">
  <p id="description">This survey is to help give feedback on how I am doing as a husband and father and how I might improve.</p>
  <form id="survey-form">
  <div class="labels">
    <label id="name-label" for="name"> Name </label>
    <div class="rightTab">
     <input type="text" name="name" id="name" placeholder="Enter Name" class="input-field" required>
    </div>
  </div>
    <br>
  <div class="labels">
    <label id="email-label" for="email"> E-mail </label>
    <div class="rightTab">
    <input type="email" name="email" id="email" placeholder="Enter E-Mail" class="input-field" required>
    </div>
  </div>
  <br>
  <div class="labels">
    <label id="number-label"> Age </label>
    <div class="rightTab">
  <input type="number" name="age" id="number" placeholder="Age" min="1" max="150" class="input-field" required>
    </div>
  </div>
  <br>
  <div class="labels">
    <label for="dropdown"> What is your relation?</label>
  </div>
    <div class="rightTab">
    <select id="dropdown" class="dropdown">
      <option disabled value>Select an option</option>
      <option value="wife"> Wife </option>
      <option value="son"> Son </option>
      <option value="daughter"> Daughter </option>
  <option value="other"> Other </option>
    </select>
  </div>
  <div class="labels">
    <label for="rating"> How have I done as a husband/father? </label>
    </div>
    <div class="rightTab">
      <ul style="list-style: none;">
      <li class="radio"><label> Amazing <input name="radio-buttons" type="radio" value="1" class="userRatings"></label>
      </li>
      <li class="radio"><label> Pretty Good <input name="radio-buttons" type="radio" value="2" class="userRatings"></label>
      </li>
      <li class="radio"><label> OK <input name="radio-buttons" type="radio" value="3" class="userRatings"></label>
      </li>
      <li class="radio"><label> Could Do Better <input name="radio-buttons" type="radio" value="4" class="userRatings"></label>
      </li>
      <li class="radio"><label> Pretty Terrible <input name="radio-buttons" type="radio" value="5" class="userRatings"></label>
      </li>
    </ul>
  </div>
  <br>
  <div class="labels">
    <label for="attributes"> What areas do I need to improve on?<br> Select all that apply</label>
  </div>
  <div class="rightTab">
    <ul style="list-style: none;">
      <li class="checkbox"><label> Spend more time with me <input name="checkboxes" type="checkbox" value="1" class="userRatings"></label>
      </li>
      <li class="checkbox"><label> Cook More <input name="checkboxes" type="checkbox" value="2"></label>
      </li>
      <li class="checkbox"><label> Work less <input name="checkboxes" type="checkbox" value="3"></label>
      </li>
    <li class="checkbox"><label> Do more projects around house <input name="checkboxes" type="checkbox" value="4"></label>
    </li>
  </div>
  <div class="labels">
    <label for="comments"> What additional ways can I improve?</label>
  </div>
  <div class="rightTab">
    <textarea id="comments" style="height:50px; width: 200px;" name="comment" placeholder="Additional suggestions here..."></textarea>
  </div>
  <button type="submit" id="submit">Submit</button> 
</form>
</div>
