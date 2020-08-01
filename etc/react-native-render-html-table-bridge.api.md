## API Report File for "react-native-render-html-table-bridge"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { Component } from 'react';
import { ComponentType } from 'react';
import { HTMLNode } from 'react-native-render-html';
import { HTMLTableProps as HTMLTableProps_2 } from '@src/types';
import { RendererDeclaration } from 'react-native-render-html';
import { StyleProp } from 'react-native';
import { TableStyleSpecs as TableStyleSpecs_2 } from '@src/types';
import { ViewStyle } from 'react-native';

// @public
export function alterNode(node: HTMLNode): void;

// @public
export function cssRulesFromSpecs(specs?: TableStyleSpecs_2): string;

// @public
export const defaultTableStylesSpecs: TableStyleSpecs_2;

// @public (undocumented)
export class HTMLTable<WVP> extends Component<HTMLTableProps_2<WVP>> {
}

// @public (undocumented)
export interface HTMLTableBaseProps {
    html: string;
    onLinkPress?: (url: string) => void;
    renderersProps: any;
}

// @public (undocumented)
export interface HTMLTableProps<WVP> extends TableConfig<WVP>, HTMLTablePropsWithStats {
}

// @public (undocumented)
export interface HTMLTablePropsWithStats extends HTMLTableBaseProps, HTMLTableStatProps {
}

// @public (undocumented)
export interface HTMLTableStatProps {
    numOfChars: number;
    numOfColumns: number;
    numOfRows: number;
}

// @public (undocumented)
export const IGNORED_TAGS: string[];

// @public (undocumented)
export function makeCustomTableRenderer(TableComponent: ComponentType<HTMLTablePropsWithStats>): RendererDeclaration;

// @public
export function makeTableRenderer(tableConfig: TableConfig): RendererDeclaration;

// @public (undocumented)
export const TABLE_TAGS: string[];

// @public
export interface TableConfig<WebViewProps = any> {
    autoheight?: boolean;
    cssRules?: string;
    defaultHeight?: number;
    maxHeight?: number;
    sourceBaseUrl?: string;
    style?: StyleProp<ViewStyle>;
    tableStyleSpecs?: TableStyleSpecs;
    transitionDuration?: number;
    useLayoutAnimations?: boolean;
    WebViewComponent: ComponentType<WebViewProps>;
    webViewProps?: WebViewProps;
}

// @public
export interface TableStyleSpecs {
    borderWidthPx: number;
    cellPaddingEm: number;
    fitContainerHeight: boolean;
    fitContainerWidth: boolean;
    fontFamily: string;
    fontSizePx: number | null;
    linkColor: string;
    selectableText: boolean;
    tdBorderColor: string;
    thBorderColor: string;
    thEvenBackground: string;
    thEvenColor: string;
    thOddBackground: string;
    thOddColor: string;
    trEvenBackground: string;
    trEvenColor: string;
    trOddBackground: string;
    trOddColor: string;
}


// (No @packageDocumentation comment for this package)

```