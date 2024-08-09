[
  {
      "nome": "Teste Start",
      "email": "start@challenge.com"
  },
  {
      "nome": "Fulano de Tal",
      "email": "fulano@qa.com"
  },
  {
      "nome": "Carlos João",
      "email": "carlosjoao@qa.com"
  },
  {
      "nome": "Ghost Silva",
      "email": "ghost_silva@fantasma.com"
  },
  {
      "nome": "Peter Parker",
      "email": "peterparker@marvel.com"
  },
  {
      "nome": "Maria Aparecida",
      "email": "mariaaparecida@qa.com"
  },
  {
      "nome": "Sebastião Levi Nunes",
      "email": "sebastiao123@teste.com"
  },
  {
      "nome": "Maitê Giovana Regina Lopes",
      "email": "maite-lopes90@outershoes.com.br"
  },
  {
      "nome": "Filipe Renato Ribeiro",
      "email": "filipe.renato.ribeiro@cdcd.com.br"
  },
  {
      "nome": "Lucca Ryan Jesus",
      "email": "lucca_ryan_jesus@imoveisvillani.com.br"
  },
  {
      "nome": "Raimunda Luana Fabiana Nascimento",
      "email": "raimunda-nascimento98@cressem.com.br"
  },
  {
      "nome": "Luana Marina Araújo",
      "email": "luana-araujo72@expressotaubate.com.br"
  },
  {
      "nome": "Bruce Wayne",
      "email": "brucewayne@gothan.com"
  },
  {
      "nome": "Carla Mariah dos Santos",
      "email": "carla_dossantos@ept.com.br"
  },
  {
      "nome": "Jennifer Agatha Pires",
      "email": "jennifer.agatha.pires@macroengenharia.com",
  },
  {
      "nome": "Luan Anderson Gonçalves",
      "email": "luan_goncalves@moncoes.com.br"
  }
]


[
  {
      "nome": "teste",
      "categoria": "start",
      "preco": 10,
      "descricao": "Start Challenge."
  },
  {
      "nome": "batata",
      "categoria": "frutas",
      "preco": 10,
      "descricao": "Batata rosa."
  },
  {
      "nome": "adesivo",
      "categoria": "utilitários",
      "preco": 0,
      "descricao": "desivo com precificação para produtos."
  },
  {
      "nome": "caneca",
      "categoria": "utilitários",
      "preco": 0,
      "descricao": "Caneca para café."
  },
  {
      "nome": "caneca chopp",
      "categoria": "utilitários",
      "preco": 25.50,
      "descricao": ""
  },
  {
      "nome": "copo grande térmico",
      "categoria": "utilitários",
      "preco": 35.90,
      "descricao": ""
  },
  {
      "nome": "mouse gamer",
      "categoria": "games",
      "preco": 101,
      "descricao": "Mouse com leds."
  },
  {
      "nome": "teclado gamer",
      "categoria": "games",
      "preco": 99,
      "descricao": "Teclado com leds."
  },
  {
      "nome": "monitor gamer",
      "categoria": "games",
      "preco": 1500,
      "descricao": "Monitor grande para jogar."
  },
  {
      "nome": "jogo batman",
      "categoria": "games",
      "preco": 150,
      "descricao": "Jogo do Batman para PC."
  },
  {
      "nome": "jogo tomb raider",
      "categoria": "games",
      "preco": 100,
      "descricao": "Jogo Tomb Raider para PC."
  },
  {
      "nome": "jogo spider-man",
      "categoria": "games",
      "preco": 200,
      "descricao": "Jogo Spider-man para PS4."
  },
  {
      "nome": "jogo pac-man",
      "categoria": "games",
      "preco": 180,
      "descricao": "Jogo Pac-man para Xbox One."
  },
  {
      "nome": "guarda-roupas lady bug",
      "categoria": "casa",
      "preco": 2500,
      "descricao": "Guarda-roupas gigante da Lady Bug."
  },
  {
      "nome": "cama solteiro",
      "categoria": "casa",
      "preco": 1800,
      "descricao": "Cama box solteiro."
  }
]



db.usuarios.countDocuments()

db.usuarios.updateOne({ nome: "Teste Start" }, { $set: { nome: "Teste Finish" } })

db.usuarios.find({ nome: "Bruce Wayne" })

db.usuarios.find({ email: "ghost_silva@fantasma.com" })

db.usuarios.deleteOne({ email: "peterparker@marvel.com" })



db.produtos.find({ descricao: "" })

db.produtos.find({ categoria: "games" })

db.produtos.find({ preco: 0 })

db.produtos.find({ preco: { $gt: 100.00 } })

db.produtos.find({ preco: { $gte: 1000.00, $lte: 2000.00 } })

db.produtos.find({ nome: /jogo/i })
