<html>
    <head>Predict Winner</head>
    <body>
        <h1>Enter the teams below</h1>
        <form action="{{  url_for('predict')}}" method="post">
            <div>
                <label>The</label>
                <input type="text" name="year1" required="required" placeholder="Year">
                <input type="text" name="team1" required="required" placeholder="Team">
            </div>
            <h2>vs</h2>
            <div>
                <label>The</label>
                <input type="text" name="year2" required="required" placeholder="Year">
                <input type="text" name="team2" required="required" placeholder="Team">
            </div>
            <div>
                <button type="submit"> Predict</button>
            </div>
        </form>
        <br>
        <br>
        {{  prediction_text  }}
    </body>
</html>
