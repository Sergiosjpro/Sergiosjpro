import tkinter as tk
ventana = tk.Tk()
ventana.title('Menú desplegable')
ventana.geometry('800x400')
barra_menu = tk.Menu(ventana)
ventana.config(menu=barra_menu)
menu_principal = tk.Menu(barra_menu)
barra_menu.add_cascade(label =
'Principal', menu=menu_principal)
submenu = tk.Menu(menu_principal)
menu_principal.add_cascade(label =
'Cartelera', menu=submenu)
submenu.add_command(label = 'Pelicula1')
submenu.add_command(label = 'Pelicula2')
submenu.add_command(label = 'Pelicula3')
submenu = tk.Menu(menu_principal)
menu_principal.add_cascade(label =
'Horarios', menu=submenu)
submenu.add_command(label = 'Películas 2D')
submenu.add_command(label = 'Películas 3D')


menu_precios = tk.Menu(barra_menu)
barra_menu.add_cascade(label =
'Precios', menu=menu_precios)
submenu = tk.Menu(menu_precios)
menu_precios.add_cascade(label =
'Películas', menu=submenu)
submenu.add_command(label = '2D')
submenu.add_command(label = '3D')
submenu = tk.Menu(menu_precios)
menu_precios.add_cascade(label =
'Bar', menu=submenu)
submenu.add_command(label = 'Combo Individual')
submenu.add_command(label = 'Combo Familiar')

menu_comprar = tk.Menu(barra_menu)
barra_menu.add_cascade(label =
'Comprar', menu=menu_comprar)

ventana.mainloop()
