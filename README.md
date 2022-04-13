# Controle_de_Series_e_Filmes
# Ainda vou colocar em um framework mas  de qualquer forma resolvi colocar os comandos que usei. 
-- Banco de dados: `movies-controll`
--

-- --------------------------------------------------------

--
-- Estrutura da tabela `movies`
--

DROP TABLE IF EXISTS `movies`;
CREATE TABLE IF NOT EXISTS `movies` (
  `id` int NOT NULL AUTO_INCREMENT,
  `type` int NOT NULL,
  `name` varchar(30) NOT NULL,
  `total_ep` int DEFAULT NULL,
  `atual_ep` int DEFAULT NULL,
  `last_view` datetime DEFAULT CURRENT_TIMESTAMP,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=6 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;

--
-- Extraindo dados da tabela `movies`
--

INSERT INTO `movies` (`id`, `type`, `name`, `total_ep`, `atual_ep`, `last_view`) VALUES
(1, 0, 'Friends', 10, 1, '2022-04-13 10:53:16'),
(2, 1, 'Avengers', NULL, NULL, '2022-04-13 10:53:16'),
(3, 1, 'Crepúsculo', NULL, NULL, '2022-04-13 11:09:48'),
(4, 0, 'Pacificador', 8, 8, '2022-04-13 11:33:48'),
(5, 1, 'A vida secreta de Walter Mitty', NULL, NULL, '2022-04-13 11:33:48');
COMMIT;
