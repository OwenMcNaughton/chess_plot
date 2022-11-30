import chess
import chess.pgn
import matplotlib.pyplot as plt
   
   
def uci_to_line(uci):
    x1 = uci.from_square % 8
    y1 = uci.from_square // 8
    x2 = uci.to_square % 8
    y2 = uci.to_square // 8
    return [x1, x2], [y1, y2]
   
   
def draw_line(uci):
    a, b = uci_to_line(uci)
    plt.plot(a, b, linewidth=4, color="r", alpha=0.5)
   
   
   
def plot_game(game, fna
    plt.clf()
   
    board = game.board()
    for move in game.mainline_move:
        draw_line(move)
   
    plt.savefig(fname)
   
   
   
pgn = open("games.pgn")
iter = 0
while True:
    game = chess.pgn.read_game(pgn)
    plot_game(game, f"{iter}.png")
    iter += 1