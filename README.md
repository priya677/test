<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="UTF-8" />
		<meta name="description" content="Play the classic Stone Paper Scissors game online." />
		<meta name="keywords" content="Stone, Paper, Scissors, Game, Play, Strategy, Fun, Online" />
		<meta name="author" content="Adiya Sharma" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
		<link rel="icon" type="image" href="./assets/images/favicon.png" />
		<link rel="preconnect" href="https://fonts.googleapis.com" />
		<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
		<link
			href="https://fonts.googleapis.com/css2?family=DM+Sans:opsz@9..40&family=Delius+Unicase&family=Inter&family=Silkscreen&display=swap"
			rel="stylesheet"
		/>
		<link rel="stylesheet" href="style1.css" />
		<title>Stone Paper Scissors Game</title>
	</head>
	<body>
		<!-- loading -->
		<section class="loading">
			

			<p>Preparing your experience</p>
		</section>

		<!-- score board -->
		<div class="topBar">
			<div class="scoreBoard">
				<div class="scoreBoard__left">
					<h1>Rock</h1>
					<h1>Paper</h1>
					<h1>Scissors</h1>
				</div>
				<div class="scoreBoard__right">
					<div class="scoreBoard__right-pc">
						<p>
							Computer<br />
							Score
						</p>
						<span id="pcScoreBoard">0</span>
					</div>
					<div class="scoreBoard__right-user">
						<p>Your <br />Score</p>
						<span id="userScoreBoard">0</span>
					</div>
				</div>
			</div>
		</div>

		<!-- Options -->
		<div class="options">
			<div class="optionsContainer">
				<!-- Stone Option -->
				<div class="circle stone" onclick="handleClick('stone')">
					<div class="ringOuter">
						<div class="ringInner">
							<div class="image">
								<img src="D:\test folder\stone.png" alt="Stone" />
							</div>
						</div>
					</div>

					<div class="rings">
						<div class="ring ripple1"></div>
						<div class="ring ripple2"></div>
						<div class="ring ripple3"></div>
					</div>
				</div>

				<!-- scissor Option -->
				<div class="circle scissor" onclick="handleClick('scissor')">
					<div class="ringOuter">
						<div class="ringInner">
							<div class="image">
								<img src="D:\test folder\scissor.png" alt="scissor"/>
							</div>
						</div>
					</div>
					<div class="rings">
						<div class="ring ripple1"></div>
						<div class="ring ripple2"></div>
						<div class="ring ripple3"></div>
					</div>
				</div>

				<!-- paper Option -->
				<div class="circle paper" onclick="handleClick('paper')">
					<div class="ringOuter">
						<div class="ringInner">
							<div class="image">
								<img src="D:\test folder\paper.png" alt="paper" />
							</div>
						</div>
					</div>
					<div class="rings">
						<div class="ring ripple1"></div>
						<div class="ring ripple2"></div>
						<div class="ring ripple3"></div>
					</div>
				</div>

				<!-- Lines -->
				<div class="line line1"></div>
				<div class="line line2"></div>
				<div class="line line3"></div>

				<div>
					<h3 id="userTagline"></h3>
				</div>
				<div>
					<h3 id="computerTagline"></h3>
				</div>
			</div>
		</div>

		<!-- RuleBook -->
		<div class="ruleBook">
			<div class="closeButton">
				<span>X</span>
			</div>
			<h1>Game Rules</h1>
			<div class="rules">
				<ul>
					<li>Rock beats scissors, scissors beat paper, and paper beats rock.</li>
					<li>
						Agree ahead of time whether you’ll count off “rock, paper, scissors, shoot”
						or just “rock, paper, scissors.”
					</li>
					<li>
						Use rock, paper, scissors to settle minor decisions or simply play to pass
						the time
					</li>
					<li>
						If both players lay down the same hand, each player lays down another hand
					</li>
				</ul>
			</div>
		</div>

		<div class="actionButtons">
			<div class="rulesButton">
				<span>rules</span>
			</div>

			<div class="nextButton">
				<a href='/resultpage'><span>next</span></a>
			</div>
		</div>

		<section class="result">
			<h1 id="result_h1">You Win</h1>
			<h2 id="result_h2">Against PC</h2>
			<span onclick="resetGame()">Play Again</span>
		</section>

		<script src="script1.js"></script>
	</body>
</html>
