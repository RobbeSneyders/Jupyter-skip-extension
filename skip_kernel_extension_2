# -*- coding: utf-8 -*-
"""
Created on Mon Apr 24 00:07:39 2017

@author: Robbe Sneyders
"""
from IPython.core.magic import (Magics, magics_class, line_cell_magic)

@magics_class
class SkipMagic(Magics):

    @line_cell_magic
    def skip(self, line, cell=None):
        '''Skips execution of the current line/cell.'''
        if eval(line):
            return
            
        ip.ex(cell)

ip = get_ipython()
ip.register_magics(SkipMagic)
