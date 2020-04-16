<img alt="GoStack" src="https://storage.googleapis.com/golden-wind/bootcamp-gostack/header-desafios.png" />

<h3 align="center">
  Challenge 05: First Node.js Project
</h3>

<p align="center">
  <a href="#rocket-about-the-challenge">About the Challenge</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#routes">Routes</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#installation">Installation</a>
</p>

## :rocket: About the Challenge

Application that stores incoming and outgoing financial transactions. It allows the registration and listing of these transactions.

### Routes

- **`POST /transactions`**

```json
{
  "id": "uuid",
  "title": "title",
  "value": 3000,
  "type": "income"
}
```

- **`GET /transactions`**

```json
{
  "transactions": [
    {
      "id": "uuid",
      "title": "Freelance",
      "value": 4000,
      "type": "income"
    },
    {
      "id": "uuid",
      "title": "Salary",
      "value": 2000,
      "type": "income"
    },
    {
      "id": "uuid",
      "title": "Payment",
      "value": 4000,
      "type": "outcome"
    },
    {
      "id": "uuid",
      "title": "Product Lorem",
      "value": 1200,
      "type": "outcome"
    }
  ],
  "balance": {
    "income": 6000,
    "outcome": 5200,
    "total": 800
  }
}
```

Within **balance**, income is the sum of all transaction values ​​with `type` income. The outcome is the sum of all transaction values ​​with `type` outcome, and the total is the value of `income - outcome`.

## Installation

1. Clone the repository: `git@github.com:matheus-neves/challenge-nodejs-fundamentals.git`
2. Access the directory: `cd challenge-nodejs-fundamentals`
3. Install the dependencies: `yarn`
4. Run the server: `yarn dev:server`
5. Server running in `http://localhost:3333/`


## :memo: License

This challenge is under license from MIT. See the archive [LICENSE](https://github.com/Rocketseat/bootcamp-gostack-desafios/blob/master/LICENSE) for more details.

---
Challenge completed ✔️by Matheus Neves and created with 💜by Rocketseat 👋 [Join the community!](https://discordapp.com/invite/gCRAFhc)
