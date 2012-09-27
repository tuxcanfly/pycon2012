# -*- Mode: Python; coding: utf-8; indent-tabs-mode: nil; tab-width: 4 -*-
### BEGIN LICENSE
# This file is in the public domain
### END LICENSE

import gettext
from gettext import gettext as _
gettext.textdomain('hello')

from gi.repository import Gtk # pylint: disable=E0611
import logging
logger = logging.getLogger('hello')

from hello_lib import Window
from hello.AboutHelloDialog import AboutHelloDialog
from hello.PreferencesHelloDialog import PreferencesHelloDialog

# See hello_lib.Window.py for more details about how this class works
class HelloWindow(Window):
    __gtype_name__ = "HelloWindow"
    
    def finish_initializing(self, builder): # pylint: disable=E1002
        """Set up the main window"""
        super(HelloWindow, self).finish_initializing(builder)

        self.AboutDialog = AboutHelloDialog
        self.PreferencesDialog = PreferencesHelloDialog

        # Code for other initialization actions should be added here.

